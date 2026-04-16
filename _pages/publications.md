---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 2
_styles: >
  .bibliography { list-style: none !important; padding-left: 0 !important; }
  .bibliography li { list-style-type: none !important; }
  .bibliography li::before { content: none !important; }
  h2 { margin-top: 2.5rem; padding-top: 1.5rem; border-top: 2px solid #ddd; }
  h2:first-of-type { margin-top: 0; padding-top: 0; border-top: none; }
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

## Working Papers

{% bibliography --query @*[category=pre-prints] %}

## Peer-Reviewed Publications

{% bibliography --query @*[category=peer-reviewed] %}

## Policy Papers

{% bibliography --query @*[category=policy-papers] %}
