---
layout: default
title: Publications
permalink: /publications/
---

<div class="page publications-page">

  <h1>Publications</h1>


  <h2>Journal Articles</h2>

  {% for pub in site.data.publications.journal %}

  <div class="publication-entry">

    <div class="publication-image">

      <img
        src="{{ pub.image | relative_url }}"
        alt="{{ pub.title }}"
      >

    </div>


    <div class="publication-info">

      <div class="publication-title">
        {{ pub.title }}
      </div>

      <div class="publication-authors">
        {{ pub.authors }}
      </div>

      <div class="publication-venue">
        {{ pub.venue }}
      </div>

      <div class="publication-links">

        {% for link in pub.links %}

          <a
            href="{{ link.url }}"
            target="_blank"
            rel="noopener noreferrer"
          >
            [{{ link.label }}]
          </a>

        {% endfor %}

      </div>

    </div>

  </div>

  {% endfor %}



  <h2>Preprints</h2>

  {% for pub in site.data.publications.preprint %}

  <div class="publication-entry">

    <div class="publication-image">

      <img
        src="{{ pub.image | relative_url }}"
        alt="{{ pub.title }}"
      >

    </div>


    <div class="publication-info">

      <div class="publication-title">
        {{ pub.title }}
      </div>

      <div class="publication-authors">
        {{ pub.authors }}
      </div>

      <div class="publication-venue">
        {{ pub.venue }}
      </div>

      <div class="publication-links">

        {% for link in pub.links %}

          <a
            href="{{ link.url }}"
            target="_blank"
            rel="noopener noreferrer"
          >
            [{{ link.label }}]
          </a>

        {% endfor %}

      </div>

    </div>

  </div>

  {% endfor %}

</div>
