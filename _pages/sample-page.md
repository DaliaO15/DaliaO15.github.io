---
title: "My work"
permalink: /sample-page/
layout: splash
author_profile: true
classes: wide

# Section Title
intro:
  - excerpt: "## My Current Work"

# Feature Row - Current Projects
feature_row:
  - image_path: /assets/img/myself.jpeg
    alt: "Project 1"
    title: "Automatic reading of handwritten letters"
    excerpt: "A project in collaboration with the University Library."
    url: /about-page/
    btn_label: "Learn More"
    image_width: "20px"
  - image_path: /assets/img/myself.jpeg
    alt: "Project 2"
    title: "My Python programming course"
    excerpt: "A collaborative project with Uppsala University and WASP-ED"
    url: /about-page/
    btn_label: "Learn More"
    image_width: "20px"

# Past Projects Ordered by Year
past_projects:
  2024:
    - title: "Project Alpha"
      description: "A project on AI and automation."
      url: /project-alpha/
    - title: "Project Beta"
      description: "A collaborative effort in data science."
      url: /project-beta/
  2023:
    - title: "Project Gamma"
      description: "A research study on machine learning."
      url: /project-gamma/
  2022:
    - title: "Project Delta"
      description: "A web development initiative."
      url: /project-delta/
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="feature_row" type="grid" %}

## Past Projects

{% for year in page.past_projects %}
### {{ year[0] }}
{% for project in year[1] %}
- [{{ project.title }}]({{ project.link }}): {{ project.description }}
{% endfor %}
{% endfor %}

