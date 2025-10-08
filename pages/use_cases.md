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
        The goal of the reGon project is to bring our tools and datasets into practical application. They are tested in 
        five use cases carried out in close collaboration with practice partners. Together, we define scenario 
        assumptions and validate the results, ensuring that our partners’ requirements are directly reflected in the 
        usability and functionality of the tools.
      </p>
    </div>
  </section>

  <section class="use-cases__items row row__wrap">

    {% include _use_cases.html %}

  </section>

  <section class="use-cases__details row row__wrap">
    {% for uc in site.data._use_cases %}
        <div class="use-cases__detail" id="{{ uc.id }}">
          <div class="use-cases__detail-heading">
            <h3>{{ uc.name }} - {{ uc.title }}</h3>
          </div>
          <div class="use-cases__description-content">
            {{ uc.description }}
            
            {% if uc.research_question %}
              <h4>Research Questions:</h4>
              {% if uc.research_question.first %}
                <ul>
                {% for question in uc.research_question %}
                  <li>{{ question }}</li>
                {% endfor %}
                </ul>
              {% else %}
                <p>{{ uc.research_question }}</p>
              {% endif %}
            {% endif %}
          </div>
          <div class="use-cases__detail-partners">
            {% if uc.industrial_partners %}
            <h4>Industrial Partners:</h4>
            {{ uc.industrial_partners }}
            {% endif %}
          </div>
            <h4>Scientific Lead: </h4>
          <div class="use-cases__detail-lead">
            {% assign scientific_lead_name = uc.scientific_lead %}
            {% assign matched_lead = site.data._partners | where: "name", scientific_lead_name | first %}

            {% if matched_lead %}
              <img src="{{ site.url }}{{ site.baseurl }}/images/{{ matched_lead.logo }}" alt="{{ matched_lead.name }} Logo" class="scientific_lead-logo" />
            {% else %}
              <p><em>No scientific lead logo found</em></p>
            {% endif %}
          </div>
        </div>
    {% endfor %}
  </section>

</div>
