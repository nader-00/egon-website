---
layout: startpage
title: "Tools & Data"
permalink: "/tools_data/"
header: no
---


<div class="page__wrap tools-data">

  <section class="tools-data__header row row__wrap">
    <div class="columns">
      <div class="tools-data__subheading">
        <p>Several open-source tools have been developed in the context of the open-eGo and eGo<sup>n</sup> projects, forming a 
coherent toolchain that now serves as the foundation for reGo<sup>n</sup>.</p>
        <div class="columns tools-data__img">
          <picture>
            <source srcset="../images/Toolchain_web_desktop.png" media="(min-width: 641px)">
            <img srcset="../images/Toolchain_web_mobile.svg" alt="Toolchain representing the relationship between the 
                various models and applications">
          </picture>
        </div>
        <p>Our energy system and grid models are built with eGo<sup>n</sup>-data and ding0. For grid analysis and planning, we use 
           the modular tools eTraGo (transmission grid) and eDisGo (distribution grid). These can be applied 
           independently or combined within the inter-grid-level planning tool eGo, which enables the investigation 
           of viable grid expansion scenarios.</p>
        <p>All input data, models, and results from these tools are published as open data on the Open Energy Platform 
           <a href="https://openenergy-platform.org/">(OEP)</a>, while the tools themselves are openly available on 
           <a href="https://github.com/openego">GitHub</a>.</p>.
      </div>     
    </div>
  </section>

  <section class="tools-data__tools row row__wrap tools">
    <div class="columns tools-data__tools-heading">
      <h2>Our Tools</h2>
    </div>
    <div class="columns tools-data__tools-text">
      <p>
      Within open_eGo, we've created a family of three grid planning tools for integrated modeling of transmission and distribution grid level:
    </p>
    </div>
    {% include _tools.html %}
  </section>

  <section class="tools-data__tools row row__wrap data">
    <div class="columns tools-data__tools-heading">
      <h2>Our Data</h2>
    </div>
    <div class="columns tools-data__tools-text">
      <p>
      Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
    </p>
    </div>
  </section>

  <div class="tools-data__oep-container row row__wrap">
    <section class="tools-data__oep columns medium-6">
      <div class="tools-data__oep-logo">
        <img src="{{ site.url }}{{ site.baseurl }}/images/webapp.png" alt="eGon WebApp">
      </div>
      <div class="tools-data__oep-content">
        <h2 class="tools-data__oep-heading">WebApp</h2>
        <p class="tools-data__oep-text">
          Explore the data and results in our WebApp
        </p>
        <div class="tools-data__oep-btn">
          <a href="https://egon.rl-institut.de" class="button">Visit WebApp</a>
        </div>
      </div>
    </section>

    <section class="tools-data__oep columns medium-6">
      <div class="tools-data__oep-logo">
        <img src="{{ site.url }}{{ site.baseurl }}/images/OEP_logo.svg" alt="OpenEnergyPlatform">
      </div>
      <div class="tools-data__oep-content">
        <h2 class="tools-data__oep-heading">Open&shy;Energy&shy;Platform</h2>
        <p class="tools-data__oep-text">
          The OpenEnergyPlatform is an open-data platform used by energy researchers to publish data in an accessible manner.
        </p>
        <div class="tools-data__oep-btn">
          <a href="https://openenergy-platform.org/" class="button">Visit OEP</a>
        </div>
      </div>
    </section>
  </div>

</div>





