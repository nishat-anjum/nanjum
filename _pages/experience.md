---
layout: page
permalink: /experience/
title: Experience
description: Industrial Affiliations, Work Experience and Responsibilities
nav: true
nav_order: 2
---

<section class="content-section">
    <strong><h4 class="resume-item-title" itemprop="name">Technical Experties</h4></strong>
    <!-- On rows -->
    <strong>Language:</strong>&nbsp; Java, Python, C/C++, JavaScript, TypeScript, R <br>
    <strong>Frameworks:</strong>&nbsp; Spring [Boot, MVC, Webflow, Security, Data JPA, Batch, Hateoas, GraphQL], Python Flask, Angular, Hibernate, JPA, Mockito<br>
    <strong>Web Services:</strong>&nbsp; REST, SOAP<br>
    <strong>Middlewares:</strong>&nbsp; WebLogic, WildFly, Tomcat, TomcatEE, Glassfish<br>
    <strong>Databases:</strong>&nbsp; MySQL, Oracle, PostgreSQL, In‑memory database Redis, Cloud Storage ‑ Minio<br>
    <strong>Tools:</strong>&nbsp; Maven, Gradle, Ant, Postman, Git, Bitbucket, Docker<br>
    <strong>OS Platforms:</strong>&nbsp; Linux, Windows, Mac<br>
    <strong>Big Data:</strong>&nbsp; Kafka, Apache KUDU, Apache Spark, Apache Druid, Elasticsearch<br>
</section>

<br>
<hr>
<br>

<section class="content-section">
        {% for job in site.data.experience %}
          <div class="resume-item" itemscope itemprop="worksFor" itemtype="http://schema.org/Organization">
                <strong><h4 class="resume-item-title" itemprop="name">{{ job.company }}</h4></strong>
                <h5 class="resume-item-details" itemprop="description">{{ job.position }} &bull; {{ job.duration }}</h5>
                <!-- <p class="resume-item-copy">{{ job.summary }}</p> -->
                    <ul>
                    {% for collection in job.responsibilities %}
                        <li>{{ collection }}</li>
                    {% endfor %}
                    </ul>
            </div>
            <hr>
        {% endfor %}

</section>
