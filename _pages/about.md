---
layout: single
title: "Junteng Liu"
permalink: /
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a first-year PhD candidate in Computer Science at the Hong Kong University of Science and Technology (HKUST), working in the HKUST NLP Group under the supervision of Prof. Junxian He. I received my B.Eng. from Shanghai Jiao Tong University (SJTU) in June 2024, where I was awarded the Zhiyuan Honor Scholarship. My research lies at the intersection of natural language processing and machine learning, with a focus on large language models: how they reason, how truthful and interpretable they are, and how hallucination arises in vision-language models.

Research Interests
======
* **LLM Reasoning and Reinforcement Learning** - large-scale synthesis of verifiable reasoning data for logical reasoning, and reinforcement learning for reasoning.
* **Hallucination in Vision-Language Models** - diagnosing perception bottlenecks, in particular for chart understanding.
* **LLM Truthfulness and Interpretability** - internal representation perspectives on truthfulness and hallucination mitigation.

Education
======
* **Ph.D. in Computer Science**, Hong Kong University of Science and Technology, 2024 - Present
* **B.Eng.**, Shanghai Jiao Tong University, 2020 - 2024
  * Zhiyuan Honor Scholarship

Research Experience
======
* **Research Intern**, MINIMAX, February 2025 - Present
* **Research Intern**, Tencent WXG, June 2024 - September 2024
  * Supervisor: Zifei Shan
* **Research Intern**, Shanghai AI Lab, June 2023 - December 2023
  * Supervisor: Prof. Yu Cheng

Publications
======

{% include base_path %}

{% if site.author.googlescholar %}
<div class="wordwrap">A complete and up-to-date list of my publications can also be found on <a href="{{ site.author.googlescholar }}">my Google Scholar profile</a>.</div>
{% endif %}

{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

Skills
======
* **Reasoning data synthesis** - scaling the synthesis of verifiable reasoning data for logical reasoning.
* **Vision-language model analysis** - perceptual bottleneck analysis in vision-language models for chart understanding.
* **Interpretability and truthfulness** - mechanistic study of truthfulness hyperplanes and in-context sharpness as hallucination alerts.
* **Benchmarking and evaluation** - design of large-scale, multi-level, multi-discipline evaluation suites for foundation models.
* **Parameter-efficient adaptation** - composing parameter-efficient modules with arithmetic operations.

Contact
======
* **Email:** jliugi@connect.ust.hk
* **GitHub:** [Vicent0205](https://github.com/Vicent0205)
* **Google Scholar:** [profile](https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate)
* **X (Twitter):** [@junteng88716710](https://twitter.com/junteng88716710)
