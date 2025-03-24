---
title: "My work"
permalink: /sample-page/
layout: splash
intro: 
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin.'
feature_row:
  - image_path: /assets/img/myself.jpeg
    alt: "placeholder image 1"
    title: "Automatic reading of handwritten letters"
    excerpt: "A project in collaboration with the University Library."
    actions:
    url: /about-page/
    btn_label: "Read More"
  - image_path: /assets/img/myself.jpeg
    alt: "placeholder image 2"
    title: "My Python course"
    excerpt: "A collaborative project with Uppsala University and WASP-ED"
    url: /about-page/
    btn_label: "Read More"
    btn_class: "btn--black"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="feature_row" type="center" %}
