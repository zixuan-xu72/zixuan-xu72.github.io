---
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
  - /teaching/
---

<div class="page-card" markdown="1">

{% comment %}The download link appears once the PDF is committed at this path.{% endcomment %}
{% assign cv_pdf = site.static_files | where: "path", "/files/Zixuan_Xu_CV.pdf" | first %}
{% if cv_pdf %}
<p class="cv-download"><a href="{{ cv_pdf.path | relative_url }}"><i class="fas fa-file-pdf" aria-hidden="true"></i> Download CV (PDF)</a></p>
{% endif %}

**Research areas:** Human-Centered AI · Human–Machine Interaction · Adaptive AI Assistance · Safety-Aware Multimodal Reasoning · Human–Autonomy Coordination

## Education

<ul class="dated-list dated-list--wide">
  <li><span class="dated-list__date">2023 – 2027</span><span class="dated-list__text"><strong>Ph.D. in Transportation</strong>, Korea Advanced Institute of Science and Technology (KAIST)<br><span class="dated-list__meta">Cho Chun Shik Graduate School of Mobility · Advisor: Prof. Tiantian (Nicole) Chen · Expected June 2027</span></span></li>
  <li><span class="dated-list__date">2022 – 2023</span><span class="dated-list__text"><strong>M.S. in Data-Driven Modeling</strong>, The Hong Kong University of Science and Technology (HKUST)<br><span class="dated-list__meta">Department of Physics and Mathematics</span></span></li>
  <li><span class="dated-list__date">2018 – 2022</span><span class="dated-list__text"><strong>B.E. in Traffic Engineering</strong>, Tongji University<br><span class="dated-list__meta">College of Transportation · Minor in Traffic Design, Management, and Control</span></span></li>
</ul>

## Research Experience

<ul class="dated-list dated-list--wide">
  <li><span class="dated-list__date">2026 – present</span><div class="dated-list__text"><strong>Visiting Ph.D. Student</strong>, <a href="https://mobility.mit.edu/">JTL Urban Mobility Lab</a>, Massachusetts Institute of Technology (MIT)<br><span class="dated-list__meta">Department of Urban Studies and Planning · Host: Prof. Jinhua Zhao · Cambridge, MA, USA</span>
    <ul class="cv-bullets">
      <li>Investigating human responses to autonomous vehicles and their implications for interaction and coordination in mixed traffic.</li>
    </ul></div></li>
  <li><span class="dated-list__date">2023 – present</span><div class="dated-list__text"><strong>Ph.D. Student Researcher</strong>, <a href="https://human-facts.kaist.ac.kr/">HumanFACTS Lab</a>, KAIST<br><span class="dated-list__meta">Cho Chun Shik Graduate School of Mobility · Daejeon, South Korea</span>
    <ul class="cv-bullets">
      <li><strong>Personalized AI assistance.</strong> Developed an LLM-based driver-assistance agent integrating driver profiles, traffic context, and retrieval to generate personalized multimodal warnings.</li>
      <li><strong>Human-in-the-loop evaluation (ongoing).</strong> Conducting a driving-simulator study comparing AI-generated and conventional warnings, measuring driver attention, situation awareness, and driving behavior.</li>
      <li><strong>Ethical AI evaluation.</strong> Examined LLM decision patterns in autonomous-vehicle ethical dilemmas and compared them with human moral preferences.</li>
      <li><strong>Research synthesis.</strong> Led a PRISMA-guided review of 68 studies on LLM-enabled automotive HMI and proposed the MODEL–REASON–ACT framework.</li>
    </ul></div></li>
</ul>

## Publications

{% assign pubs = site.publications | sort: "date" | reverse %}
{% for category in site.publication_category %}
{% assign category_pubs = pubs | where: "category", category[0] %}
{% if category_pubs.size > 0 %}
<h3>{{ category[1].title }}</h3>
<ul class="pub-list">
  {%- for pub in category_pubs %}
  {% include publication-entry.html pub=pub %}
  {%- endfor %}
</ul>
{% endif %}
{% endfor %}

## Research Projects

<ul class="dated-list dated-list--wide">
  <li><span class="dated-list__date">2026 – present</span><span class="dated-list__text"><strong>Modular Chiplet Structure-Based Human-Centered AI Foundation Models for Robust, Scalable Automated Driving</strong><br><span class="dated-list__meta">Korea Institute for Advancement of Technology (KIAT) · Korea–U.S. R&amp;D · Student Researcher</span></span></li>
  <li><span class="dated-list__date">2026 – 2029</span><span class="dated-list__text"><strong>Development of a Detachable On-Board Device for Multi-Vehicle Remote Operation and Safety Enhancement Technologies (DOVE)</strong><br><span class="dated-list__meta">Korea Planning &amp; Evaluation Institute of Industrial Technology (KEIT) · Korea–Czech R&amp;D · Student Researcher</span></span></li>
  <li><span class="dated-list__date">2024 – 2027</span><span class="dated-list__text"><strong>Empowering Mobility for a Smart Aging Society: Developing and Testing of Large Language Model-Based Driver Assistance Agent</strong><br><span class="dated-list__meta">National Research Foundation of Korea (NRF) · Lead Student Researcher</span></span></li>
  <li><span class="dated-list__date">2024 – 2026</span><span class="dated-list__text"><strong>⟨Mobility 100⟩ Sustainable Mobility in Villages: Innovative Technologies and Policies for Super-Aged Societies</strong><br><span class="dated-list__meta">KAIST Strategic Initiative for Super-Aged Society · Lead Student Researcher</span></span></li>
</ul>

## Honors & Awards

{% include awards-list.html wide=true %}

## Talks

{% include talks-list.html wide=true %}

## Teaching

<ul class="dated-list dated-list--wide">
  <li><span class="dated-list__date">Spring 2025</span><span class="dated-list__text"><strong>Teaching Assistant</strong>, MO.60010: Traffic Safety (graduate elective)<br><span class="dated-list__meta">Cho Chun Shik Graduate School of Mobility, KAIST</span></span></li>
</ul>

## Academic Service

- **Journal reviewer:** Transportation Research Part A: Policy and Practice; Travel Behaviour and Society; IEEE Transactions on Vehicular Technology; IEEE Open Journal of Intelligent Transportation Systems
- **Conference reviewer:** IEEE Intelligent Transportation Systems Conference (ITSC); IEEE Intelligent Vehicles Symposium (IV)

## Technical Skills

- **Programming:** Python, C#, R
- **AI / ML:** PyTorch, Hugging Face, LLMs and VLMs, fine-tuning (LoRA, QLoRA), RL post-training (GRPO), ms-swift, vLLM
- **AI systems:** LLM agents, retrieval-augmented generation (RAG), LangChain, multimodal inference
- **Simulation:** Unity (driving-simulator development), Autoware
- **Research tools:** Linux, Git, Jupyter, LaTeX

</div>
