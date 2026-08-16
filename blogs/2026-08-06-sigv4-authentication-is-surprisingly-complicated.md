---
title: "SigV4 authentication is surprisingly complicated"
url: "https://www.tigrisdata.com/blog/sigv4/"
date: "2026-08-06"
feed_url: "https://www.tigrisdata.com/blog/rss.xml"
---
SigV4 looks simple: sign a request, check the signature. Then you implement canonicalization, clock skew, and a cache that isn't allowed to hold your key.
