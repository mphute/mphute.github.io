---
layout: home
title: Home
---

<div id="intro-wrapper" class="l-middle">
	<div id="intro-title-wrapper">
		<div id="intro-image-wrapper">
			<img id="intro-image" src="images/portrait.png"></div>
		<div id="intro-title-text-wrapper">
			<h1 id="intro-title">Hi, I'm Mansi Phute</h1>
			<div id="intro-subtitle">CS PhD at Georgia Tech</div>
			<div id="intro-title-socials">
				{% for link in site.data.social-links %}
					{% if link.on-homepage == true %}
						{% include social-link.html link=link %}
					{% endif %}
				{% endfor %}
			</div>
		</div>
	</div>
	<!-- <hr class="l-middle home-hr"> -->
	<div id="everything-else" class="l-middle">
		<a href="{{ site.url }}/cv"><div><i class="fa fa-portrait icon icon-right-space"></i>CV</div></a>
		<a href="{{ site.url }}/projects"><div><i class="fa fa-shapes icon icon-right-space"></i>Projects</div></a>
		<a href="{{ site.url }}/everything-else"><div><i class="fa fa-list-ul icon icon-right-space"></i>Everything Else</div></a>
	</div>
	<div>
		My research focuses on the <b>security</b> and <b>explainability</b> of multimodal foundation models. I work on developing explanations for ML systems, analyzing them to identify vulnerabilities, and finding solutions to mitigate these issues.
		My work spans a wide range of application areas, including multi-object robust tracking in computer vision, developing defenses against attacks on large language models, and understanding large language models and the insights they can give us into human interactions.
	</div>
	<div style="height: 0.5rem"></div>
	<div>
		I am currently a PhD student at Georgia Tech with <a href="http://www.cc.gatech.edu/~dchau/">Polo Chau</a> as a part of the <a href="http://poloclub.gatech.edu">Polo Club of Data Science</a>.
		<br>
	</div>
	<div style="height: 1rem"></div>
	<div>
		I have collaborated with designers, developers, and scientists at <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/intellabs.svg"> Intel Labs, <img class="intro-logo" style="width: 18px; padding-bottom: 3px;" src="/images/ntu.svg"> Nanyang Technological University, and <img class="intro-logo" style="width: 24px;" src="/images/dassault_logo_small.svg"> Dassault Systems.
	</div>
</div>


<hr class="l-middle home-hr">

<h2 class="feature-title l-middle"> Featured Publications </h2>
<div style="height: 1rem"></div>
<div class=" -1-col l-page">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' | reverse %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>

<div style="height: 4rem"></div>

<!-- <h2 class="feature-title l-middle">
	<a href="{{ site.url }}/everything-else" style="color: #303030">Everything Else</a>
</h2>
<div style="height: 1rem"></div>
<div id="everything-else" class="l-middle">
	<a href="{{ site.url }}/projects"><div>All Projects</div></a>
	<a href="{{ site.url }}/blog"><div>Blogs</div></a>
    <a href="{{ site.url }}/tools"><div>Tools</div></a>
</div> -->


[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"

<!-- <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/poloclub.png"> <a href="http://poloclub.gatech.edu">Polo Club of Data Science</a> -->

<!-- I have strong interests in building reliable algorithms and toolkits that understand, fortify and democratize AI security with an eye towards scalability and practicality in real-world settings.  -->

<!-- , with an emphasis on enhancing deep learning algorithm safety and explainability. I achieve this through methods of architecture modification, multi-task learning, and visualizing model behavior under adversarial attacks. My work also spans application domains such as multimodal systems, object detection, object tracking, table representation learning, and structural health monitoring. -->


<!-- In general, I have strong interests in creating scalable, efficient, and robust multimodal models.
scalable and practical AI security algorithms and toolkits. -->
