---
layout: default
title: Locating Session ID
parent: Managing Captures
nav_order: 3
---

# Locating the Session ID
{: .no_toc }

Each resource in a collection originates from a capture session.
The Session ID of the parent Capture Session from which a resource originates is shown in:
1. the Session ID column in resources view
2. the metadata inspector when a resource is selected

[diagram]

Clicking on the resource’s Session ID will take you to the [Session Manager](), where you may then [delete]() or [download]() that specific session as a WARC.

#### **Proceed with Caution**
{: .label .label-red }
Deleting a session permanently removes **ALL** resources captured during that session.
{: 	.bg-yellow-100 .p-4}
