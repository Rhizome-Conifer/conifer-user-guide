---
layout: default
title: Contribute
nav_order: 11
---
# Contributing To This Guide

Have any requests, suggested edits or topics you would like to add to this guide?

The guide is [managed on GitHub](https://github.com/Rhizome-Conifer/conifer-user-guide) and you can [open an issue](https://github.com/Rhizome-Conifer/conifer-user-guide/issues) to make a suggestion. Contributions via pull requests are also welcome.

If you’re unfamiliar with GitHub, please feel free to write to us directly at [support@conifer.rhizome.org](mailto:support@conifer.rhizome.org) with any feedback.


#### Current and Past Contributors to the Conifer User Guide

<ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul>
