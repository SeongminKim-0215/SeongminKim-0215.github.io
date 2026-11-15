---
layout: page
permalink: /publications/
title: Publications
description: "† equal contribution, * corresponding author."
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<!-- Filter by authorship. Hidden until the script runs, so it never shows as a dead control. -->
<div class="pub-filter" role="group" aria-label="Filter publications by authorship" hidden>
  <button type="button" data-filter="all" aria-pressed="true">All</button>
  <button type="button" data-filter="first" aria-pressed="false">First authorship</button>
  <button type="button" data-filter="co" aria-pressed="false">Co-authorship</button>
</div>

<!-- One list for everything. Under-review papers (@unpublished) sit first in
     papers.bib, so they lead their year; within a year, file order is page order. -->
<div class="publications" id="published">

{% bibliography --query @* %}

</div>

<!-- Inlined rather than linked. As a separate file the script was cached on its own
     URL, so a browser could pair fresh markup with a stale copy of it: the numbering
     shipped and did not appear for anyone who had loaded this page before. Inline, it
     cannot go stale independently of the page that uses it.

     The canonical source is `_includes/pubfilter.js`. `assets/js/pubfilter.js` still
     builds from that same include, so the old URL keeps working for anyone holding
     markup that still links it; without that they would 404 and lose the filter bar
     altogether, which is worse than the bug this change fixes. -->
<script>
  {%- include pubfilter.js -%}
</script>
