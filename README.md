# 🐈 AffiliCats Microsites

This repo shows the concept of using [microsites](https://en.wikipedia.org/wiki/Microsite)
to pre-warm the cache of a full Progressive Web App (PWA) using regular HTML and AMP HTML.

Related repo: https://github.com/googlechromelabs/affilicats/.

Note that for the AMP sample to work, the AMP microsite needs to be on the same origin
as the PWA, else the service worker installation process will be stopped by the current
AMP logic (related [issue](https://github.com/ampproject/amphtml/issues/18055))
with the error message below:

```
data-iframe-src (https://googlechromelabs.github.io) should be a URL on the same origin as the source
(https://tomayac.github.io) or canonical URL (https://tomayac.github.io) of the AMP-document.

Uncaught (in promise) Resource: failed to build: amp-install-serviceworker#1: data-iframe-src
(https://googlechromelabs.github.io) should be a URL on the same origin as the source
(https://tomayac.github.io) or canonical URL (https://tomayac.github.io) of the AMP-document.
```

<img width="400" src="https://github.com/tomayac/affilicats-microsites/blob/master/serp.png" alt="Search Engine Results Page showing the microsites">
