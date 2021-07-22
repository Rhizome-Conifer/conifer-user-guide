---
layout: default
title: FAQs
nav_order: 10
---

# Frequently Asked Questions
{: .no_toc }

We advise all users to make themselves familiar with the introductory sections of this user guide, [Intro: The Challenge at Hand](../challenges/) and [How Conifer Works](../how-it-works/), which covers some technical basics about web archiving with Conifer.
{: .fs-6 .fw-300 }


## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---


## Why can’t I just delete a single page?
Browsers often present web pages as a single object that is accessible via a URL. However, in reality, a single web page consists of many artifacts, each of them with their own URL, that are loaded in parallel or sequence, or dependent on user interaction. This effectively means that pages do not have clearly determined, universal boundaries as objects.

Additionally, many of the artifacts loaded to support a page, such as a logo image that appears on many locations throughout a website, cannot be clearly connected to a single page. However, such an artifact might exactly be the reason why you want to delete a page.

If you want to have full control of your collection’s contents on a page level, you can plan to capture every page in its own session. However, for web sites that use certain technical patterns for navigation, this might make it impossible to fluidly navigate the captured version.


## Can I export or backup my collections?
Yes, you may backup a collection by [downloading it as a warc file](../manage-sessions/exporting-warc/).

## Why can’t I successfully patch a page?
Patching works by trying to load resources that have not been captured in a previous session. The idea is that the boundary of a capture, which has been created in the past, is expanded with newly captured artifacts. However this process fails if the web resource the patch is based on, typically a web page captured earlier, has changed too much since that original capture.

This can easily happen with frequently updated pages such as social media profiles, blogs, or news sites. Some web pages are technically different each time they are accessed, even if no changes are visible in the browser.

If such changes are following a reproducible pattern, it might be possible to improve Conifer so that patching could work better for them. Please [file a bug report](../report-bug/) if you encounter patching issues.

<!-- ## What are some best practices when capturing pages?


## Why doesn’t my captured page look or behave as expected? -->


---
**Have a question?** Contact us at [support@conifer.rhizome.org](mailto:support@conifer.rhizome.org).
{: .fs-4 .fw-300 }
