---
layout: page
title: About Me
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}** :wave:,<br>
I am currently studying the last year of my degree in computer engineering at UC3M, during my years in the career I have discovered my passion for cybersecurity, so every day I focus on continuing to acquire knowledge in both network team and blue team. In constant growth and learning, I participate in CTFs to expand and improve my skills in this field.

<div class="row">
<h2 class="mb-3">Contact Info</h2>
	<div class="row justify-content-between align-items-center">
    <div class="col-10">
      <p class="mb-1">Mobile</p>
    </div>
    <div class="col-2 text-right">
      <p class="mb-1 text-muted">+34 677 14 68 48</p>
    </div>
  </div>
  <div class="row justify-content-between align-items-center">
    <div class="col-10">
      <p class="mb-1">Email</p>
    </div>
    <div class="col-2 text-right">
      <p class="mb-1 text-muted">albertolinarescorrales16@gmail.com</p>
    </div>
  </div>
</div>

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Network Security Tools" source=site.data.security-skills %}
</div>

<div class="row">
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
{% include about/skills.html title="Idioms" source=site.data.Idioms %}
</div>

<div class="row">
    <div class ="col-lg">
        <h2 class ="mb-3">Work Experience</h2>
        {% include about/timeline.html%}
    </div>
</div>

<div class="row">
    <div class ="col-lg">
        <h2 class ="mb-3">Education</h2>
        {% include about/timeline-education.html%}
    </div>
</div>

<div class="row">
    <div class ="col-lg">
        <h2 class ="mb-3">Licences and certifications</h2>
        {% include about/timeline-lic.html%}
    </div>
</div>
