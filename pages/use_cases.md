---
layout: startpage
title: "Use Cases"
permalink: "/use_cases/"
header: no
---

<div class="page__wrap use-cases">

  <section class="use-cases__header row row__wrap">
    <div class="columns">
      <p class="use-cases__subheading">
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
      </p>
    </div>
  </section>

  <section class="use-cases__items row row__wrap">

    {% include _use_cases.html %}

  </section>

  <section class="use-cases__details row row__wrap">
    {% for uc in site.data._use_cases %}
      <div class="columns" id="{{ uc.id }}">
        <div class="use-cases__detail">
          <div class="use-cases__detail-heading">
            <h3>{{ uc.name }}</h3>
          </div>
          <div class="use-cases__detail-content">
            {{ uc.research_question }}
          </div>
          <div class="use-cases__detail-partner">
            {% assign partner_name = uc.partner %}
            {% assign matched_partner = site.data._partners | where: "name", partner_name | first %}

            {% if matched_partner %}
              <img src="{{ site.url }}{{ site.baseurl }}/images/{{ matched_partner.logo }}" alt="{{ matched_partner.name }} Logo" class="partner-logo" />
            {% else %}
              <p><em>No partner logo found</em></p>
            {% endif %}
          </div>
        </div>
      </div>
    {% endfor %}
  </section>

</div>