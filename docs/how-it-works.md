---
layout: default
title: How Conifer Works
nav_order: 03
---

# How Conifer Works
{: .no_toc }

Conifer allows you to capture web sites by routing the traffic in between your browser and the web through the Conifer server. When anyone accesses a capture, they are able to engage with the site as it existed. Below, we will define some fundamental concepts to help ensure successful captures.
{: .fs-6 .fw-300 }

### Capture and Access in Conifer
Many web sites today are not just made of static files that need to be downloaded, but include complex scripts that determine what happens on a page while users are visting. Web pages do not load in one go, but gradually unfold as you interact with them.

Instead of thinking about the web as remote files, Conifer works with **sessions**. During a session, requests sent by the browser and responses from the web are **captured** while you are interacting with sites. Sessions are the smallest unit of data in Conifer. A **collection** typically contains multiple captured sessions.

When a captured session is **accessed**, or viewed online, Conifer makes the browser request resources from the collection instead of the live web. Viewers of a collection should be able to repeat any action during access that were performed during capture.  
