---
layout: home
title: Home
---

<div>
<a href="https://mansiphute.com">
<!-- <img class="title-logo" src="/images/apw_logo.svg"> -->
</a>
</div>

<h1 class="intro-title">Mansi Phute</h1>

<!-- {% include nav.html %} -->

<div class="intro">
	
	<div class="intro-text">
		<p markdown="1">
		Hello! I’m an MS student in the [College of Computing][coc] at [Georgia Tech][gt]. I'm a member of the [Polo Club of Data Science][poloclub] advised by [Polo Chau][poloclub]. 
		</p>
		<p markdown="1">
       My research in **Adversarial ML** in developing effective defences against adversarial attacks. I am interested in .
		</p>
		<p markdown="1">
		I have collaborated with researchers and developed solutions for the following institutions:  
		<img class="intro-logo" style="width: 100px; padding-bottom: 10px;" src="/images/intellabs.svg">
		<img class="intro-logo" style="width: 100px; padding-bottom: 10px;" src="/images/.svg">
		</p>
	</div>

    <div class="intro-image">
      <img src="/images/portrait.jpg" style="border-radius: 4px;">

      <div class="intro-image-links">
    	{% for link in site.data.social-links %}
    	{% if link.on-homepage == true %}
    	{% include social-link.html link=link %}
    	{% endif %}
    	{% endfor %}
    </div>

    <div class="intro-cv-wrapper">
    	<a href="/cv" style="color: #515151">
    	<span class="intro-cv">
    	Here's my CV.
    	</span></a>
    </div>

    </div>

</div>

<!-- <div style="padding-top:15px;"></div> -->

<hr style="margin-left: 0;">
<div class="cover-wrapper">
	<div class="cover-side">
		Featured <a href="/cv#publications" style="color: #303030"><strong>Research Publications</strong></a>
	</div>
{% assign sortedPublications = site.data.publications | sort: 'feature-order' %}
{% for feature in sortedPublications %}
{% if feature.featured == true %}

{% include feature.html feature=feature %}

{% endif %}
{% endfor %}

</div>

[about]: {{ site.url }}/about
[projects]: {{ site.url }}/projects
[archive]: {{ site.url }}/archive "Archive."

[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computer Science"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau."
[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
