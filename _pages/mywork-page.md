---
title: "My work"
permalink: /mywork-page/
layout: splash

# Section Title
intro:
  - excerpt: "## What I am currently doing:"

# Feature Row - Current Projects
feature_row:
  - image_path: /assets/img/handwrittenletter.jpg
    alt: "Project 1"
    title: "Automatic Reading of Handwritten Historical Letters"
    excerpt: "This is a project in collaboration with the University Library, focusing on historical text analysis. It has four main parts: handwritten text recognition, translation (from 1700s Swedish to English), summarization, and NER. To tackle this, I’m using a mix of computer vision and language models.
    "
  - image_path: /assets/img/mypythoncourse.jpg
    alt: "Project 2"
    title: "My Python Programming Lifelong Learning Course"
    excerpt: "A collaborative project with Uppsala University and WASP-ED. The course is designed to help students learn how to use Python libraries effectively. I decided to focus on libraries for scientific programming and data analysis, giving students practical tools to work with real-world data."
  - image_path: /assets/img/example_plot.png
    alt: "Project 3"
    title: "VKontakte Scraper"
    excerpt: "A data collection tool built in collaboration with the Dept. of Informatics and Media at UU. I developed the first-ever bulk VKontakte web scraper for extracting data from a non-Western social media platform, making large-scale data collection more efficient and accessible."
    

# Past Projects Ordered by Year
past_projects:
  2025:
    - title: "Version control workshop"
      description: "Led an introductory workshop on version control with Git and GitHub"
      link: "https://www.uu.se/centrum/digital-humaniora-och-samhallsvetenskap/kalendarium/arkiv/2025-03-19-introduction-to-version-control-with-git--github"
    - title: "X-QUEST"
      description: "In this project I worked with image analysis and OCR to digitalise pictures of periodicals."
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

{% include feature_row %}

## Past Projects and Participation

{% for year in page.past_projects %}
### {{ year[0] }}
{% for project in year[1] %}
- [{{ project.title }}]({{ project.link }}): {{ project.description }}
{% endfor %}
{% endfor %}

