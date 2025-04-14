---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
<p>
  <a href="{{ site.baseurl }}/files/Ralston_CV_2025.pdf" target="_blank" rel="noopener">
    Download CV (PDF)
  </a>
</p>

{% include base_path %}

Education
======
* Ph.D in Economics, University of California Irvine, 2018
* B.S. in Mathematics and Economics, University of Kansas, 2013

Work experience
======
* August 2020 - Present: Assistant Professor
  * Department of Economics
  * Whitman College

* July 2018 - June 2020: Postdocotoral Research Associate
  * Department of Economics
  * Hankamer Business School
  * Baylor University

Publications
======

<h3>Published Papers</h3>
<ul>
{% assign published = site.publications | where: "status", "published" | reverse %}
{% for post in published %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

<h3>Submitted Papers</h3>
<ul>
{% assign submitted = site.publications | where: "status", "submitted" | reverse %}
{% for post in submitted %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

<h3>Works in Progress</h3>
<ul>
{% assign wip = site.publications | where: "status", "wip" | reverse %}
{% for post in wip %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
