---
layout: default
title: How Conifer Works
nav_order: 3
---

# How Conifer Works
{: .no_toc }

To archive a website, Conifer allows you to capture the site and your interaction with it.  When anyone accesses a capture session, they are able to engage with the site as it existed. Below, we will define some fundamental concepts to help ensure successful captures.
{: .fs-6 .fw-300 }

### Capture and Access in Conifer
Many web sites today are not made of static files, but include complex scripts and interactions. Web pages do not load in one go, but gradually unfold as you interact with them.

Instead of thinking about the web as files, Conifer works with **sessions**. During a session, requests sent by the browser and responses from the web are **captured** while you are interacting with sites. Sessions are the smallest unit of data in Conifer. A **collection** typically contains multiple captured sessions.

When a captured session is **accessed**, or viewed online, Conifer makes the browser request resources from the collection (which contains captured Conifer sessions) instead of the live web. You should be able to repeat any action during access that you performed during capture.  
