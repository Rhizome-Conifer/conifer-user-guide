---
layout: page
title: Search
published: true
nav_order: 9
nav_exclude: true
---

# Collection Search

![Searchbox dropdown](/assets/images/search-dropdown.png)

## Using

Conifer’s search feature provides multiple ways to dig deeper into your collections. The search box is located at the top of the page on the [Collection Manager](https://guide.conifer.rhizome.org/docs/ui-overview/#collection-manager) page.

The default configuration searches by the webpage content type identified by the `is:page` prefix. To expand the search options, click the triangle at the right side of the search box.


### Advanced Search
Within the search dropdown you’ll find multiple ways to narrow the search parameters.

**Contains the words** - Searches within either the title of the capture or the full-text of each capture (see [full-text search](#full-text-search)).

**URL contains** - This searches only in the url of the capture or asset in the case of file type searches.

**Include File Types** - Limits results to captured elements from the selected mime types.

**Date Archived** - Restrict results between a certain date range or recording session.

### Search Query Composition

Search query configurations are reflected in the prefix applied to the search box. Search queries can also be built or modified by hand with this system.

<figure>
  <img src="{{site.url}}/assets/images/filter-demo.gif" alt="Filtering demo"/>
  <figcaption class="text-small">An example search query for images with “gif” in the url between may 25 2019 - may 25 2020</figcaption>
</figure>

## Full-Text Search

<figure>
  <img src="{{site.url}}/assets/images/search-indexing.gif" alt="Filtering demo"/>
  <figcaption class="text-small">Search indexing indicator</figcaption>
</figure>

[Conifer Supporters](https://supporter.conifer.rhizome.org) gain access to an even more expansive search tool with Full-Text Search indexed with Solr. Full-Text search not only searches within URLs and titles from the pages you capture, but also includes the text content of the pages themselves -- at improved speeds.

<figure>
  <img src="{{site.url}}/assets/images/search-demo.gif" alt="Filtering demo"/>
  <figcaption class="text-small">Demo of full-text search</figcaption>
</figure>
