---
layout: page
title: Autopilot
published: true
nav_order: 8
---

# Autopilot

## Using

Autopilot can perform actions on the current web page loaded in Conifer, similar to a human user. It can be activated via the Autopilot button on the top right during capture. When the button is solid green, a *specialized behavior* is available for the current web page. A white button indicates that only the *default behavior* will be presented instead.

A specialized behavior performs actions specific to the currently presented website.

The default behavior tries to perform generally useful actions: scrolling down and triggering play  embedded media.

Click the Autopilot button to bring up the Autopilot panel. Pick one from the presented behaviors and run it with the Start button below.

![Autopilot Initial](/assets/autopilot-start.png)

While the behavior is running, you cannot interact with the page. The Autopilot displays information on the current capturing process. Once the behavior concludes or is manually terminated, you can continue with manual capture.

![Autopilot Running](/assets/autopilot-running.png)


## For best results

Autopilot is performing complex actions on web pages. We offer the following recommendations for best results:

- Start Autopilot soon after a page loads, to avoid getting Autopilot confused.

- Autopilot is available in both native browsers as well as in remote browsers that have the Autopilot capability listed. We recommend using the latest available version of Chrome, as we do the most thorough testing with that browser. If your local browser is not supported, pick a remote browser from the browser menu.
  ![Browser Dropdown](/assets/browser-dropdown.png)

- For *Local Browsers:* Most browsers aggressively limit any activity happening in background tabs or minimized windows. Keep the tab that Autopilot is running in at the front, or place it into a new window. Do not minimize windows in which Autopilot is running.

- *Remote Browsers* are not affected by running in a background tab, but can only be active for 60 minutes at most. If the tab with a remote browser is closed, the Autopilot will stop after 10 minutes.

- The behavior’s description will contain hints on how you can improve capture, for instance by logging in to a site through Conifer.

## Caveats

- For many sites, getting “all” content will not be possible, especially when large amounts of items are presented via infinite scrolling. Many web sites are not able to be scrolled all the way to the bottom, but will enforce a limit earlier in the process.

- Like Conifer overall, Autopilot is a [“best-effort” approach](../challenges/): Sites may not be captured fully for a variety of reasons, such as rate limiting, unexpected network issues, and so forth. Autopilot's status messages and status log will help explain what has happened and how much content was captured.

- Web sites can be expected to be frequently redesigned or technically re-architectured. When such an updated happens, Autopilot behaviors probably won’t continue working as planned and need to be adapted. Each behavior lists a date when it was last updated.

- At the moment, Autopilot works on single web pages. If you see the URL changing during a behavior’s execution, Autopilot didn’t navigate to a new page, but the web site’s functionality itself changed the display of the URL to represent its current state. Since such URLs are also linkable from the "outside" of the web page, Conifer makes an attempt to request that outside view in the background and makes that into a bookmark.

## Troubleshooting

- If you run into issues with Autopilot, please try again after switching in between remote and native browser, and/or at a later time to make sure the error is occuring consistently.

- Often times, a site may change in subtle ways that requires a behavior to be updated. Please don’t hesitate to inform us about behaviors becoming outdated, especially if you think a site has recently updated.

- Feel free to email us at <support@conifer.rhizome.org> and if possible include the behavior’s status log and any other useful information.

## Available behaviors

At the moment, the following specialized behaviors are available:
- Instagram user account
- SoundCloud User Account
- Twitter timeline
- YouTube
- SlideShare
- Facebook timeline

For more detailed information on the behavior system, currently available behaviors and how they're created, please see our new [Webrecorder Behaviors Developer Docs](https://webrecorder.github.io/behaviors).

Have a request for a custom behavior? Please open an issue on the [webrecorder/behaviors](https://github.com/webrecorder/behaviors) repository, or email us at <support@conifer.rhizome.org>.
