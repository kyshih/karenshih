---
layout: page
title: about # this will be tab title
permalink: /
nav: true
---

<img class="col one right" src="{{ site.baseurl }}/assets/img/prof_pic.jpg">

<br/>
I am a PhD student in the Biology department at <a href="https://profiles.stanford.edu/karen-shih" target="blank">Stanford</a>. I am co-advised by <a href="https://petrovlab-stanford.squarespace.com" target="blank">Dmitri Petrov</a> and <a href="https://med.stanford.edu/winslowlab.html" target="blank">Monte Winslow</a>. We study cancer evolution using tumor barcoding, CRISPR/Cas9-mediated gene editing and deep sequencing in mouse models. With this technique, we aim to investigate the fitness landscape of tumor suppression in lung adenocarcinoma under different intracellular or 
extracellular environments.

In my free time, I like social dancing, skiing, playing board games, and lifting.

<a href="{{ site.baseurl }}/assets/cv.pdf" target="_blank" style="font-size: smaller;">CV</a>

<!-- Write your biography here. Tell the world about yourself. Link to your favorite <a href="http://reddit.com" target="blank">subreddit</a>. You can put a picture in, too. The code is already in, just name your picture "prof_pic.jpg" and put it in the img folder. 

Link to your social media connections, too. This theme is set up to use <a href="http://fortawesome.github.io/Font-Awesome/" target="blank">Font Awesome icons</a>, like the ones below. Add your facebook, twitter, linkedin, or just disable all of them.  -->


<br/>
<br/>
<hr/>
<br/>
<div class="contacticon center">
    {%- if site.email -%}
	<a href="mailto:{{ site.email }}"><i class="fa fa-envelope-square"></i></a>
    {% endif %}
    {%- if site.github_username -%}
	<a href="https://github.com/{{ site.github_username }}" target="_blank"><i class="fa-brands fa-square-github"></i></a>
    {% endif %}
    {%- if site.linkedin_username -%}
	<a href="https://www.linkedin.com/in/{{ site.linkedin_username }}" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
    {% endif %}
    {%- if site.twitter_username -%}
	<a href="https://twitter.com/{{ site.twitter_username }}" target="_blank"><i class="fa-brands fa-square-x-twitter"></i></a>
    {% endif %}
    {%- if site.google_scholar_username -%}
    <a href="https://scholar.google.com/{{ site.google_scholar_username }}" target="_blank"><i class="fa-brands fa-google"></i></a>
    {% endif %}
</div>

<div class="col three caption">
	Feel free to reach me via email.
</div>
