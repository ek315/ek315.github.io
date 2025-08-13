---
layout: page
permalink: /publications/
title: "publications & projects"
nav: true
nav_order: 2
---

{% assign page.title = nil %}

{% include bib_search.liquid %}

<div class="publications">

  <h2 class="pub-category">Journal & Conference Publications</h2>
  {% bibliography --template bib_custom --query @*[category=publications] --sort_by year --order descending %}

  <h2 class="pub-category">Class Projects</h2>
  {% bibliography --template bib_custom --query @*[category=class] --sort_by year --order descending %}

  <h2 class="pub-category">Patents</h2>
  {% bibliography --template bib_custom --query @*[category=patents] --sort_by year --order descending %}

  <h2 class="pub-category">Other</h2>
  {% bibliography --template bib_custom --query @*[category=other] --sort_by year --order descending %}

</div>
