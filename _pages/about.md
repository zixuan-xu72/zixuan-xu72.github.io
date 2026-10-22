---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<section class="home-section home-section--intro" markdown="1">

## <span class="section-icon"><i class="fa-solid fa-user" aria-hidden="true"></i></span>About

I am a **Ph.D. candidate at KAIST**, advised by [Prof. Tiantian Chen](https://sites.google.com/view/chentiantian/home), and currently a **Visiting Student Researcher at MIT**, working with [Prof. Jinhua Zhao](https://mobility.mit.edu/people/jinhua-zhao/).
{: .lead}

My research focuses on **human-centered AI for intelligent and autonomous systems**. I develop adaptive, safety-aware AI assistance that accounts for human needs and environmental context, primarily using intelligent vehicles as a research setting. Beyond system design, I investigate how people interpret and respond to AI, including its implications for human judgment, reliance, and behavior. Building on this work, I am extending my research toward **human–autonomy coordination**, exploring how interactions between people and autonomous agents may shape broader mobility systems.

<div class="postdoc-callout">
  <div class="postdoc-callout__body">
    <p class="postdoc-callout__tag"><span class="postdoc-callout__dot" aria-hidden="true"></span>Open to work</p>
    <p class="postdoc-callout__title">I am seeking postdoctoral opportunities starting in Fall 2027.</p>
    <p class="postdoc-callout__text">Happy to connect about human-centered AI, human–AI interaction, and human–autonomy coordination.</p>
  </div>
  <div class="postdoc-callout__actions">
    <a class="postdoc-callout__btn" href="mailto:zixuan72@mit.edu"><i class="fa-solid fa-envelope" aria-hidden="true"></i> Email</a>
    <a class="postdoc-callout__btn" href="/cv/"><i class="fa-solid fa-file-lines" aria-hidden="true"></i> CV</a>
  </div>
</div>

</section>

<section class="home-section" markdown="1">

## <span class="section-icon"><i class="fa-solid fa-flask" aria-hidden="true"></i></span>Research

My research spans three connected levels: **designing adaptive AI systems, understanding human responses, and investigating interactions at scale.**
{: .section-intro}

<div class="research-grid">
  <div class="research-card research-card--1">
    <span class="research-card__icon"><i class="fa-solid fa-shield-heart" aria-hidden="true"></i></span>
    <p class="research-card__stage"><span class="research-card__num">01 /</span> Design</p>
    <h3 class="research-card__title">Adaptive &amp; Safety-Aware AI Assistance</h3>
    <p class="research-card__text">How can AI determine when to assist, what support to provide, and how to communicate it? I develop personalized AI agents and safety-aware multimodal reasoning methods that integrate human needs, environmental context, and risk.</p>
  </div>
  <div class="research-card research-card--2">
    <span class="research-card__icon"><i class="fa-solid fa-people-arrows" aria-hidden="true"></i></span>
    <p class="research-card__stage"><span class="research-card__num">02 /</span> Interact</p>
    <h3 class="research-card__title">Human–AI Interaction &amp; Behavioral Adaptation</h3>
    <p class="research-card__text">How do people interpret and respond to AI assistance, and when does it support human judgment? I examine the behavioral and ethical dimensions of human–AI interaction, including reliance, trust, and decision-making, with ongoing work on human-in-the-loop evaluation.</p>
  </div>
  <div class="research-card research-card--3">
    <span class="research-card__icon"><i class="fa-solid fa-city" aria-hidden="true"></i></span>
    <p class="research-card__stage"><span class="research-card__num">03 /</span> Scale <span class="research-card__badge">Emerging Direction</span></p>
    <h3 class="research-card__title">Human–Autonomy in Sociotechnical Systems</h3>
    <p class="research-card__text">How do individual interactions between people and autonomous agents develop into broader patterns of coordination and behavior? I am exploring empirically grounded simulations of human–AV interaction to examine heterogeneous human responses and coordination dynamics. In the longer term, I aim to understand how such interactions may contribute to changes in mobility systems, social expectations, and the adoption of autonomous technologies.</p>
  </div>
</div>

</section>

<section class="home-section" markdown="1">

## <span class="section-icon"><i class="fa-solid fa-book-open" aria-hidden="true"></i></span>Selected Publications

{% assign selected_pubs = site.publications | where: "selected", true | sort: "date" | reverse %}
<ul class="pub-list">
{%- for pub in selected_pubs %}
{% include publication-entry.html pub=pub %}
{%- endfor %}
</ul>

<p class="more-link"><a href="{{ '/publications/' | relative_url }}">Full publication list →</a></p>

</section>

<section class="home-section home-section--awards" markdown="1">

## <span class="section-icon"><i class="fa-solid fa-award" aria-hidden="true"></i></span>Selected Honors &amp; Awards

{% include awards-list.html selected=true %}

</section>
