---
layout: page
permalink: /experience/
title: Experience
description: Industrial Affiliations, Work Experience and Responsibilities
nav: true
nav_order: 2
---
<section class="content-section">
        {% for job in site.data.experience %}
          <div class="resume-item" itemscope itemprop="worksFor" itemtype="http://schema.org/Organization">
                <strong><h4 class="resume-item-title" itemprop="name">{{ job.company }}</h4></strong>
                <h5 class="resume-item-details" itemprop="description">{{ job.position }} &bull; {{ job.duration }}</h5>
                <p class="resume-item-copy">{{ job.summary }}</p>
                    <ul>
                    {% for collection in job.responsibilities %}
                        <li>{{ collection }}</li>
                    {% endfor %}
                    </ul>
            </div>
        {% endfor %}

</section>