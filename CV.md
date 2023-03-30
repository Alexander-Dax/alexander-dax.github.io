---
layout: cv
---

<section class="content-section">
    <header class="section-header">
        <h2>Experience</h2>
    </header>
    {% for job in site.data.experience %}
   <div class="resume-item" itemscope itemprop="worksFor" itemtype="http://schema.org/Organization">
              <h4 class="resume-item-title" itemprop="name">{{ job.company }}</h4>
              <h5 class="resume-item-details" itemprop="description">{{ job.position }} &bull; {{ job.duration }}</h5>
              <p class="resume-item-copy">{{ job.summary }}</p>
    </div><!-- end of resume-item -->
    {% endfor %}
</section>
<!-- end Experience -->

<!-- begin Education -->
<section class="content-section">
    <header class="section-header">
        <h2>Education</h2>
    </header>
    {% for education in site.data.education %}
    <div class="resume-item" itemscope itemprop="alumniOf" itemtype="http://schema.org/CollegeOrUniversity">
              <h4 class="resume-item-title" itemprop="name">{{ education.uni }}</h4>
              <h5 class="resume-item-details group" itemprop="description">{{ education.degree }} &bull; {{ education.year }}</h5>
    <p class="resume-item-copy">{{ education.summary }}</p>
    </div>
    {% endfor %}
</section>
<!-- end Education -->
 
<!-- begin Projects -->
<section class="content-section">
    <header class="section-header">
        <h2>Publications</h2>
    </header>
    {% for project in site.data.projects %}
    <div class="resume-item" itemscope itemtype="http://schema.org/CreativeWork">
              <p class="resume-item-copy">{{ project.description }}</p>
              <p class="resume-item-copy">{{ project.link }}</p>
    </div>
    {% endfor %}
</section>
<!-- end Projects -->

<!-- begin Skills -->
<section class="content-section">
    <header class="section-header">
        <h2>Skills</h2>
    </header>
            {% for skill in site.data.skills %}
            <div class="resume-item">
              <h4 class="resume-item-title">{{ skill.skill }}</h4>
              <p class="resume-item-copy">{{ skill.description }}</p>
            </div>
            {% endfor %}
</section>
<!-- end Skills -->


 <!-- begin Associations -->
<section class="content-section">
    <header class="section-header">
        <h2>Associations</h2>
    </header>
    {% for association in site.data.associations %}
    <div class="resume-item" itemscope itemprop="memberOf" itemtype="http://schema.org/Organization">
              <h4 class="resume-item-title" itemprop="name">{% if association.url %}<a class="publink" href="{{ association.url }}">{{ association.organization }}</a>{% else %}{{ association.organization }}{% endif %}</h4>
              <h5 class="resume-item-details" itemprop="description">{{ association.role }} &bull; {{ association.year }}</h5>
              <p class="resume-item-copy">{{ association.summary }}</p>
    </div>
    {% endfor %}
</section>
<!-- end Associations -->

<!-- begin Interests -->
<section class="content-section">
    <header class="section-header">
        <h2>Outside Interests</h2>
    </header>
    <div class="resume-item">
        <ul class="resume-item-list">
        {% for interest in site.data.interests %}
            <li>{{ interest.description }}</li>
        {% endfor %}
        </ul>
    </div>
</section>
<!-- end Interests -->

