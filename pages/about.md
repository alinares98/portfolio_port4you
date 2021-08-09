---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}** :wave:,<br>
I am currently studying the last year of my degree in computer engineering at UC3M, during my years in the career I have discovered my passion for cybersecurity, so every day I focus on continuing to acquire knowledge in both network team and blue team. In constant growth and learning, I participate in CTFs to expand and improve my skills in this field.

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Network Security Tools" source=site.data.security-skills %}
</div>

<div class="row">
{% include about/skills.html title="Soft Skills" source=site.data.other-skills %}
</div>

<div class="row">
    <div class ="col-lg">
        <h2 class ="mb-3">Work Experience</h2>
        <div class="col mt-4">
        <div class ="timeline-body bg-themed" style="background-color: darkgoldenrod">
        {% include about/timeline.html%}
    </div>
    </div>>
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
