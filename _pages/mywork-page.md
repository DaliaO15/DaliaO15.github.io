---
title: "My work"
permalink: /mywork-page/
layout: splash

# Section Title
intro:
  - excerpt: "# What I am currently working on:"

# Feature Row - Current Projects
feature_row:
  - image_path: /assets/img/0059.png
    alt: "Project 1"
    title: "Generative model of real human faces"
    url: "https://github.com/DaliaO15/ddpm_model_faces"
    excerpt: "This project implements a Denoising Diffusion Probabilistic Model (DDPM) to generate realistic human faces."
  - image_path: /assets/img/mypythoncourse.jpg
    alt: "Project 2"
    title: "My Python Programming Lifelong Learning Course"
    url: "https://wasp-ed.org/python/"
    excerpt: "A collaborative project with Uppsala University and WASP-ED, focused on Python libraries for scientific programming and data analysis."

# Section Title
intro_2025:
  - excerpt: "# 2025:"

# Feature Row - 2025
feature_row_2025:
  - image_path: /assets/img/handwrittenletter.jpg
    alt: "Project 1"
    title: "Automatic Reading of Handwritten Letters"
    excerpt: "It had four main parts: handwritten text recognition, translation (from 1700s Swedish to English), summarization, and NER. To tackle this, I used a mix of computer vision and language models."
  - image_path: /assets/img/version-control-sample-3.png
    alt: "Project 2"
    title: "Version control workshop"
    url: https://www.uu.se/centrum/digital-humaniora-och-samhallsvetenskap/kalendarium/arkiv/2025-03-19-introduction-to-version-control-with-git--github
    excerpt: "Led and designed an introductory workshop on version control with Git and GitHub."
  - image_path: "https://cdn4.picryl.com/photo/2019/09/05/africa-15cba9-1024.jpg"
    alt: "Project 3"
    title: "Pilot project for X-QUEST"
    excerpt: "In this project I worked with image analysis and OCR to digitalise pictures of printed periodicals from Africa."

# Section Title
intro_2024:
  - excerpt: "# 2024:"

# Feature Row - 2024
feature_row_2024:
  - image_path: /assets/img/psychotests.png
    alt: "Project 1"
    title: "HTR for psychological tests"
    excerpt: "Evaluated the applicability of cutting-edge hand written text recognition and vision large language models to extract information from physiological tests of jobseekers."
  - image_path: /assets/img/example_plot.png
    alt: "Project 2"
    title: "VKontakte web scraper"
    url: "https://github.com/DaliaO15/VK-post-scraper"
    excerpt: "I developed the first-ever bulk VKontakte web scraper for extracting data from a non-Western social media platform, making large-scale data collection more efficient and accessible."
  - image_path: /assets/img/pp_workshop.jpeg
    alt: "Project 3"
    title: "Peer programming workshop"
    excerpt: "Led and designed an internal workshop to increase the collaboration and knowledge transfer within the developers in my team."

# Section Title
intro_2023:
  - excerpt: "# 2023:"

# Feature Row - 2023
feature_row_2023:
  - image_path: /assets/img/psychotests.png
    alt: "Project 1"
    title: "Political parties logos detection model"
    excerpt: "Developed an end-to-end ML pipeline to train an object detection model for recognizing political party logos in real-life videos."
  - image_path: /assets/img/abstract_2_copy.png
    alt: "Project 1"
    title: "Tiktok scraper"
    url: "https://github.com/DaliaO15/Tiktok-scraping"
    excerpt: "Developed a data scraper for TikTok, leveraging audio transcription models and text processing to extract insights from short videos."
  - image_path: /assets/img/cup-or-glass.png
    alt: "Project 1"
    title: "Object detection workshop"
    excerpt: "Led and designed a techinical workshop about object detection with Roboflow and the YOLO family."


# Past Projects Ordered by Year
past_projects:
  2023:
    - title: "Political parties logos detection model"
      description: "Developed an end-to-end ML pipeline to train an object detection model for recognizing political party logos in real-life videos."
    - title: "Tiktok scraper" 
      description: "Developed a data scraper for TikTok, leveraging audio transcription models and text processing to extract insights from short videos."
      link: "https://github.com/DaliaO15/Tiktok-scraping"
    - title: "Object detection workshop"
      description: "Led and designed a workshop on object detection with Roboflow and the YOLO family."
  2022:
    - title: "Evaluating the Effectiveness of Active Learning Methods in Drug Repurposing"
      description: "Thesis focusing on the evaluation of active machine learning models for regression and classification in drug repurposing for Covid."
      link: "https://uu.diva-portal.org/smash/record.jsf?dswid=-6253&pid=diva2%3A1698759&c=3&searchType=SIMPLE&language=en&query=dalia+ortiz+pablo&af=%5B%5D&aq=%5B%5B%5D%5D&aq2=%5B%5B%5D%5D&aqe=%5B%5D&noOfRows=50&sortOrder=author_sort_asc&sortOrder2=title_sort_asc&onlyFullText=false&sf=all"
  2020:
    - title: "Señales de alerta temprana en modelos deterministas de Dermatis Atópica"
      description: "Contributed to and optimised existing code to analyze bifurcations in a hybrid mathematical model for Atopic Dermatitis, demonstrating critical slowing down before a rare bifurcation event and providing insights for potential early-warning indicators."
  2019:
    - title: "Señales de alerta temprana en modelos deterministas y estocásticos de sistemas biológicos"
      description: "Thesis on dynamical systems in biological processes, focusing on evaluating the applicability of bifurcation predictions for disease prevention."
      link: "132.248.9.195/ptd2019/septiembre/0796043/Index.html"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="feature_row" %}

{% include feature_row id="intro_2025" type="center" %}

{% include feature_row id="feature_row_2025" %}

{% include feature_row id="intro_2024" type="center" %}

{% include feature_row id="feature_row_2024" %}

{% include feature_row id="intro_2023" type="center" %}

{% include feature_row id="feature_row_2023" %}


## Past Projects and Participation

{% for year in page.past_projects %}
### {{ year[0] }}
{% for project in year[1] %}
- {% if project.link %} **[{{ project.title}}]({{ project.link }})** {% else %} **{{ project.title}}** {% endif %}: {{ project.description }}
{% endfor %}
{% endfor %}


