---
layout: default
title: Native vs Remote Browsers
parent: Approaches to Capturing
nav_order: 1
---

# Native vs. Remote vs. Desktop Browsers
{: .no_toc }

There are three browser options to capture a site:
{: .fs-5 .fw-300 }
- Via your **local browser**
- Via **remote browser**
- Via the **desktop app**
{: .fs-5 .fw-300 }

---

## Browser Choice Affects Capture Results
The browser you choose to capture a session will impact how the session is captured and how it will appear when accessed. There are four factors in a capture session: the browser that is operated by the user, its connection to the web archiving backend that writes the data, network location, and user identity.

The **browser** is performing all the network requests, which are captured via the Conifer backend. Anything the browser doesn't request will not be captured. This can depend on the browser’s configuration, such as an installed ad blocker or certain privacy features being activated. Additionally, browsers can differ in their overall capabilities and for instance support different image formats or JavaScript features. As a result, the same website sometimes appears differently when accessed with different browsers. It can be a source of error if a website was captured using Safari and is later accessed with Firefox, or even if different versions of the same browser.

This is true if you are using your **local browser** or a **remote browser** provided by Conifer. With a remote browser you have the opportunity to use the exact same browser for both capture and access, also in the future. Remote browsers are pre-configured browsers running in the cloud, with computing resources shared across all Conifer users. As a result, you might need to wait for one to start up for you if demand is currently high, or get network lag.

## Rewriting vs. Proxy mode

A browser can connect to the web archiving backend in two ways: **rewriting mode** or **proxy mode**.

In **rewriting mode**, all resources the browser requests are changed on the fly so that instead of reaching out to the original URL on the live web, everything goes through the web site conifer.rhizome.org. This complex process runs partly in the browser, and partly on the web archiving backend. The part running in the browser needs to be regularly updated in order to support the browser people use. In Conifer, rewriting mode is the only mode available for local browsers.

**Proxy mode** has the web archiving backend connected to the browser via web proxy. A web proxy is an intermediate server that routes traffic in between an internal network and the whole internet. The browser can make requests as usual and the web archiving backend will have access to all of them, with almost no rewriting required. This makes proxy mode generally a more stable and reliable capture method that doesn’t require constant updating. It is however not guaranteed that it leads to better results than rewriting mode. In Conifer, **proxy mode is only available for remote browsers**.

## Network Location and Site Localization
Websites can also appear differently depending on the **network location** they are accessed from. When you use Conifer to capture web sites, Conifer’s network location in an amazon datacenter in Virginia, USA, might cause the page you’re looking at to appear in a different language than you would expect, or deny access to certain items that are accessible in other parts of the world. Sites might also limit access, since every user of Conifer shares a network location with all other Conifer users who perhaps all want to capture from the same site. **Sites may also limit access due to high traffic**, since all Conifer users share one network location.

## Capturing with Desktop App
To capture from your regular network location, you can try the **[Webrecorder Desktop app](https://github.com/webrecorder/webrecorder-desktop/releases/)**, a standalone web archiving software using almost the same user interface as Conifer. This app is based on a modified Chrome browser and offers capture and access in proxy mode. Collections created with the app can also be [uploaded to Conifer](../../manage-sessions/uploading-warc).

## Capturing Logged-In Content
Many websites are personalized and appear differently depending on **user identity**. Conifer cannot know which sites you have previously logged in to on your browser. Each capture session, regardless of whether you are using your native browser or a remote one, begins without any login data. In other words, each capture session begins with the user logged out of all services.

 You may log in to websites during a session, however, **do note that your credentials may be captured as data within your collection**.
 {: 	.bg-yellow-100 .p-4}

 **Tip:** Consider using 'throwaway credentials' if you must log in to a site for a capture.

 If you need to better understand the risks of logging in to a site during a capture session, feel free to reach out to our team at [support@conifer.rhizome.org](mailto:support@conifer.rhizome.org).
