# Synchronous Speech-to-Text Recognition Overview

Synchronous recognition processes short audio clips that go up to **60 seconds**

* Sends audio data directly in the API request
* Receives the transcribed text in a single API response
* Suits quick and real-time tasks using the `recognize` endpoint (`POST /v2/{recognizer=projects/*/locations/*/recognizers/*}:recognize`)

<br>

# Synchronous 