# Speech-to-Text API Overview

Google's STT is an AI-powered service that converts spoken audio into text across over 85 languages and variants

* Uses advanced speech recognition models

<br>

# Transcription Methods

## Synchronous

Synchronous recognition processes short audio clips that go up to 60 seconds

* Sends audio data directly in the API request
* Receives the transcribed text in a single API response
* Suits quick and real-time tasks using the `recognize` endpoint (`POST /v2/{recognizer=projects/*/locations/*/recognizers/*}:recognize`)

<br>

## Asynchronous (Batch)

Batch recognition transcribes long audio files that range between minutes to hours and are stored in Cloud Storage buckets via asynchronous operations (Submits a request with a storage)

* The user submits a batch recognition request to the **batchRecognize** endpoint via `POST /v2/{recognizer}:batchRecognize` with a JSON body specifying **files[]** array containing URI fields containing the GCS URI paths for the audio files that the user wishes to transcribe

### Polling

Polling involves the user repeadly querying the operation status of the endpoint at fixed intervals

* The user will then poll the **batchRecognize** endpoint via `GET /v2/{parent=projects/*/locations/*}/operations/{operation_id}` every 5 to 30 seconds until **done: true** responses show **metadata** with progress during execution
* Each GET request should return JSON with **done: false** along with **metadata** specifying the progress of the transcription until the processing is complete
* The **response.results[]** will contain the transcripts if **inline_output_config** is specified once the transcription is complete (If **inline_output_config** isn't specified then the user will have to download the transcribed audio from a GCS URI prefix)
* Ideal for offline transcription of podcasts, videos, or meetings

<br>

### Callbacks

Callbacks involves the user enabling notifications via `notification_config` in the API request with a Pub/Sub topic name

* The API will automatically publish **Operation** update messages as JSON to the specified topic upon state changes
* The user's service should subscribe via pull/push in order to receive notifications asynchronously while also enabling event-driven processing without polling loops
* Ideal for scalable production systems that are handling many jobs

<br>

## Streaming

Streaming recognition handles real-time audio input from sources by continuously sending chunks of audio to the `streamRecognize` endpoint

* Receives interim transcriptions periodically
* Ideal for live applications with confiugrable latency via streaming config

<br>

# Recognition Models

## Chirp

<br>

## Telephony

<br>

# Service Endpoints

| Endpoint Path | Method | Purpose |
| --- | --- | --- |
| `POST /v2/{recognizer=projects/*/locations/*/recognizers/*}:recognize` | POST | Synchronous recognition for