---
permalink: /
title: About me
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I am a Ph.D. student in Computer Science at [Columbia University](https://www.columbia.edu/), where I work in the [AlQuraishi Lab (AQLab)](https://www.aqlab.io/) under the supervision of Professor [Mohammed AlQuraishi](https://www.aqlab.io/). My research focuses on <strong>deep generative models</strong>, <strong>machine learning theory</strong> and <strong>algorithms</strong>, with applications to biomolecular structure prediction.

<ul class="interests">
  <li>Deep generative models</li>
  <li>Diffusion &amp; flow matching</li>
  <li>Protein structure &amp; dynamics</li>
  <li>Machine learning theory</li>
  <li>Graph neural networks</li>
</ul>

At AQLab, I co-developed [OpenFold3](https://github.com/aqlaboratory/openfold-3), an open-source reproduction of AlphaFold3 for joint 3D modeling of proteins, nucleic acids, ligands and complexes. I also work on diffusion and flow-matching methods, with an emphasis on understanding their mode-collapse behaviour and breaking it to unlock the multiple conformations and dynamics of proteins. In this direction, I contributed to [ConforNets](https://arxiv.org/abs/2604.18559), which steers OpenFold3 toward alternative protein conformations by modulating its latent representations. In summer 2026, I was a Quantitative Researcher intern at [Optiver](https://optiver.com/) in Chicago, working on low-latency order execution.

Before Columbia, I was a Research Engineer in the [Data Science and Mining Team](http://www.lix.polytechnique.fr/dascim/) at [École Polytechnique](https://www.polytechnique.edu/en) with Professor [Michalis Vazirgiannis](http://www.lix.polytechnique.fr/~mvazirg/), where I worked on structure-aware antibiotic resistance classification with Graph Neural Networks. I hold a Master's degree in Mathematics, Computer Vision and Machine Learning (MVA) from [École Normale Supérieure Paris-Saclay](https://ens-paris-saclay.fr/) and a Diplôme d'Ingénieur in Data Science from [CentraleSupélec](https://www.centralesupelec.fr/) ([Université Paris-Saclay](https://www.universite-paris-saclay.fr/)), including an exchange semester at UT Austin. I also interned at [Amadeus](https://amadeus.com/en), forecasting demand under COVID-19 non-stationarity, and at [Institut Gustave Roussy](https://www.gustaveroussy.fr/), where I developed KmemBERT for explainable survival prediction from oncology reports.

## News

<ul class="news">
{% for item in site.data.news limit: 5 %}
  <li class="news__item"><span class="news__date">{{ item.date }}</span><span>{{ item.text }}</span></li>
{% endfor %}
</ul>
{% if site.data.news.size > 5 %}
<details class="news__older">
  <summary>Older news</summary>
  <ul class="news">
  {% for item in site.data.news offset: 5 %}
    <li class="news__item"><span class="news__date">{{ item.date }}</span><span>{{ item.text }}</span></li>
  {% endfor %}
  </ul>
</details>
{% endif %}

## Selected Publications

{% for post in site.publications reversed %}
  {% include archive-single-publication.html %}
{% endfor %}

<a class="section-more" href="{{ site.baseurl }}/publications/">All publications &rarr;</a>
