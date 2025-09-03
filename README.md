# simple-proxy

Simple reverse proxy to bypass CORS, used by [movie-web](https://movie-web.app)/[P-Stream](https://pstream.org).
Read the docs at https://docs.pstream.org/proxy/introduction

---

### features:
 - Deployable on many platforms - thanks to nitro
 - header rewrites - read and write protected headers
 - bypass CORS - always allows browser to send requests through it
 - secure it with turnstile - prevent bots from using your proxy
 - parse and bypass m3u8 stream restrictions - make sure the IP is not blocked by the CDN, may need to be on a VPS.
 - Caching of tls segments (disable with DISABLE_CACHE=true in .env)

> [!WARNING]
> Turnstile integration only works properly with cloudflare workers as platform

### supported platforms:
 - cloudflare workers
 - AWS lambda
 - nodejs
 - netlify edge functions
