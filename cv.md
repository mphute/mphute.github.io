---
layout: cv
title: CV
permalink: cv/
jsarr:
- js/scripts.js
---

<h1 id="cv-title"><a href="{{ site.url }}">Mansi Phute</a></h1>

<div style="height: 1rem"></div>
<div>
	My reserach interests are Reponsible AI and AI safety.
	I work on developing explanations for ML systems, analyzing them to identify vulnerabilities, and finding solutions to mitigate these issues.
	My UNDREAM system system offers a way to bridge differentiable rendering and photorealistic simulation for end-to-end adversarial attacks, thus enabling beter transferability of attacks to the physical world.
	My work includes LLM Self Defense, which leverages the models own understanding of harm to protect itself from attacks.
	<!-- I have worked with multimodal foundational models to create Semi-Truths, a large scale dataset that tests robustness of our current fake image detection systems on multiple axes. -->
</div>

<div class="cv-spacer"></div>

<div class="cv-spacer"></div>

<div class="cv-image-links-wrapper">
	<div class="cv-image-links">
		{% for link in site.data.social-links %}
			{% if link.cv-group == 1 %}
				{% include cv-social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
	<div class="cv-image-links">
		{% for link in site.data.social-links %}
			{% if link.cv-group == 2 %}
				{% include cv-social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
</div>

***

## Education

{::nomarkdown}
{% for degree in site.data.education %}
{% include cv/degree.html degree=degree %}
{% endfor %}
{:/}

## Research Experience

{% for experience in site.data.experiences %}
{% if experience.type == 'academic' %}
{% include cv/experience.html experience=experience %}
{% endif %}
{% endfor %}

## Industry Research Experience

{% for experience in site.data.experiences %}
{% if experience.type == 'industry' %}
{% include cv/experience.html experience=experience %}
{% endif %}
{% endfor %}


## Honors and Awards

{% for award in site.data.awards %}
{% include cv/award.html award=award %}
{% endfor %}

## Publications


{% assign selectedBoolForBibtex = false %}
{% assign journal = site.categories.papers %}
{% for pub in journal %}
{% if pub.type != "misc" %}
{% include cv/publication.html pub=pub selectedBoolForBibtex=selectedBoolForBibtex %}
{% endif %}
{% endfor %}

<!-- ## Preprint

{% assign preprint = site.categories.papers | where: 'type', "misc" %}
{% for pub in preprint %}
{% include cv/publication.html pub=pub selectedBoolForBibtex=selectedBoolForBibtex %}
{% endfor %} -->

## Talks and Presentations

{% assign talktitles = site.data.talks | group_by:"title" %}
{% for title in talktitles %}
{% include cv/talk.html talk=title %}
{% endfor %}

## Press

{% for press in site.data.press %}
{% include cv/press.html press=press %}
{% endfor %}

## Teaching

{% for teach in site.data.teaching %}
{% include cv/teaching.html teach=teach %}
{% endfor %} 

<!-- ## Grants and Funding

{% for fund in site.data.funding %}
{% include cv/fund.html fund=fund %}
{% endfor %} -->

<!-- ## Interactive Articles

{% for article in site.data.articles %}
{% include cv/article.html article=article %}
{% endfor %} -->

<!-- ## Technology Skills

{% for skill in site.data.skills %}
{% include cv/skill.html skill=skill %}
{% endfor %} -->

## Service

<!-- <div class="cv-service-title"><b>Organizer</b></div>
{% for venue in site.data.organizer %}
{% include cv/venue.html venue=venue %}
{% endfor %} -->

<!-- <div class="cv-service-title"><b>Program Commitee</b></div>
{% for venue in site.data.pc %}
{% include cv/venue.html venue=venue %}
{% endfor %} -->

<!-- <div class="cv-service-title"><b>Institutional</b></div>
{% for institution in site.data.institutional %}
{% include cv/institutional.html institution=institution %}
{% endfor %} -->

<div class="cv-service-title"><b>Reviewer</b></div>
{% for venue in site.data.reviewer %}
{% include cv/venue.html venue=venue %}
{% endfor %}

<!-- <div class="cv-service-title"><b>Member</b></div>
{% for member in site.data.memberships %}
{% include cv/member.html member=member %}
{% endfor %} -->

<!-- ## Design

{% for design in site.data.designs %}
{% include cv/design.html design=design %}
{% endfor %} -->

## Mentoring

{::nomarkdown}
{% for mentee in site.data.mentoring %}
{% include cv/mentee.html mentee=mentee %}
{% endfor %}
{:/}

## References

{% for reference in site.data.references %}
{% include cv/reference.html reference=reference %}
{% endfor %}


[cv]: {{ site.url }}/cv.pdf "My CV."

[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
[gt]: http://gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "GT Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "GT College of Computing"



<!-- I am highly self-disciplined, strong risk-taking and fearlessness about working on novel approaches. 
I got praise from my internship mentors about willingness to review technical approaches, receive and incorporate feedback, 
and ask questions until understanding about reasoning behind mentor's recommendations. 
Most importantly, my positive energy level throughout the research career is exceptional and contagious to teammates. -->


<!-- My research focuses on trustworthy machine learning, computer vision, and multimodal foundation models, with an emphasis on enhancing deep learning algorithm safety and explainability. I achieve this through methods of architecture modification, multi-task learning, and visualizing model behavior under adversarial attacks. My work also spans application domains such as multimodal systems, object detection, object tracking, table representation learning, and structural health monitoring. -->

<!-- I have strong interests in building reliable algorithms and toolkits that understand, fortify and democratize AI security with an eye towards scalability and practicality in real-world settings.  -->

