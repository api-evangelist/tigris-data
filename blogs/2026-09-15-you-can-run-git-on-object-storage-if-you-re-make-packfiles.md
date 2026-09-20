---
title: "You can run git on object storage if you re-make packfiles"
url: "https://www.tigrisdata.com/blog/objgit-packfiles/"
date: "2026-09-15"
feed_url: "https://www.tigrisdata.com/blog/rss.xml"
---
Git packfiles were designed for mmap and local disk, so pulling one object out of a bucket means guessing at a byte range. I wrote a new format instead.
