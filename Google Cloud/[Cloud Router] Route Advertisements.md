# Cloud Router Route Advertisements Overview

A Cloud Router route advertisment 

<br>

# Router Route Advertisement Level

The user chooses an advertisement mode that applies globally to all peers on the Cloud Router object

## Default Advertisement Mode

Allows users to advertise subnet ranges that are local to the VPC network

<br>

## Custom Advertisement Mode

Allows users to specify the exact CIDR ranges that will be sent in BGP updates to the peer

* Enables users to explicitly control which IP prefixes a Cloud Router announces over BGP to its peers

<br>

# BGP Session

Each BGP session can either inherit the router-level advertisement mode or be set to use its own custom set of advertised prefixes

## Default Advertisement Mode

Advertises prefixes according to the advertisement mode defined at the router level for the Cloud Router that contains the BGP session

<br>

## Custom Advertisement Mode

Allows users to specify the exact CIDR ranges that will be sent in BGP updates to the peer