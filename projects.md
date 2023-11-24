---
layout: page
title: Projects
permalink: projects/
---

Things I do, including research, academic course projects, and miscellaneous interests.

## Research

<div class="project-spacer-small"></div>

<div class="l-page project-grid">
    {% for project in site.categories.papers %}
    {% include project.html project=project %}
    {% endfor %}
</div>


<div class="project-spacer-small"></div> 

<div class="l-page project-grid">
    {% for project in site.categories.projects %}
    {% include project.html project=project %}
    {% endfor %}
</div> 
<!-- ## Course Projects

<!-- <div class="project-spacer-small"></div> -->

## Other

<ul>
<li><a href="https://github.com/mphute/mphute.github.io"><code>mphute.github.io</code> on Github</a></li>
</ul>
