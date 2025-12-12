# Cache Modes Overview

* Allows users to control the factors that determine whether Cloud CDN caches their content

<br>

# Cache Modes

## CACHE_ALL_STATIC

`CACHE_ALL_STATIC` will have Cloud CDN automatically cache successful responses with static content that isn't otherwise non-cacheable

* The default behavior for Cloud CDN-enabled backends that we created using the CLI or via REST APIs

<br>

## USE_ORIGIN_HEADERS

`USE_ORIGIN_HEADERS` will have Cloud CDN only cache responses that include valid HTTP caching directives and headers from the origin

<br>

## FORCE_CACHE_ALL

`FORCE_CACHE_ALL` will have Cloud CDN cache all successful responses while largely ignoring whether the origin marked them as cacheable or not

* Must be used carefully to avoid caching pre-user or sensitive content since it can cache responses even when they're associated with Authorization headers