# Cache Key Overview

A cache key is an identifier that determines whether a request will hit an existing cached object or require a fetch from the origin

* Each cached object at the edge is stored under a cache key derived from the request URI
* Cloud CDN will compute the cache key when a new request arrives and check to see if there's an existing entrry (If there is then you got a cache hit and the object is served from the edge)

<br>

# Custom Cache Keys

A custom cache key is a configurable definition of what parts of the HTTP request are used to uniquely identify cached objects

* Allows users to control how aggressively or granularly Cloud CDN caches responses
