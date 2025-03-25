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
    title: "Automatic Reading of Handwritten Letters"
    excerpt: "This is a project in collaboration with the University Library, focusing on historical text analysis. It has four main parts: handwritten text recognition, translation (from 1700s Swedish to English), summarization, and NER. To tackle this, I’m using a mix of computer vision and language models.
    "
  - image_path: /assets/img/mypythoncourse.jpg
    alt: "Project 2"
    title: "My Python Programming Lifelong Learning Course"
    excerpt: "A collaborative project with Uppsala University and WASP-ED. The course is designed to help students learn how to use Python libraries effectively. I decided to focus on libraries for scientific programming and data analysis, giving students practical tools to work with real-world data. The fifth round of the course started this March!"
  - image_path: /assets/img/example_plot.png
    alt: "Project 3"
    title: "VKontakte Scraper"
    excerpt: "A data collection tool built in collaboration with the Dept. of Informatics and Media at UU. I developed the first-ever bulk VKontakte web scraper for extracting data from a non-Western social media platform, making large-scale data collection more efficient and accessible."
    

# Past Projects Ordered by Year
past_projects:
  2025:
    - title: "Version control workshop"
      description: "Led and designed an introductory workshop on version control with Git and GitHub"
      link: "https://www.uu.se/centrum/digital-humaniora-och-samhallsvetenskap/kalendarium/arkiv/2025-03-19-introduction-to-version-control-with-git--github"
    - title: "Pilot project for X-QUEST"
      description: "In this project I worked with image analysis and OCR to digitalise pictures of printed periodicals from Africa."
  2024:
    - title: "HTR for psychological tests"
      description: "Evaluated the applicability of cutting-edge hand written text recognition and vision large language models to extract information from physiological tests of jobseekers."
    - title: "VKontakte web scraper (ongoing)"
      description: "Designed and created a data scraper solution to extract data from VKontakte providing, consequently, the PI with a large dataset for future engagement and text analysis."
      link: "https://github.com/DaliaO15/VK-post-scraper"
    - title: "Peer programming workshop"
      description: "Led and designed an internal workshop to increase the collaboration and knowledge transfer within the developers in my team."
    - title: "Brought a visitor from the IBERO"
      description: "Initiated a collaboration with the Ibero University in Mexico that led to the visit of a PhD student to the CDHU at Uppsala University."
  2023:
    - title: "Political parties logos detection model"
      description: "Developed an end-to-end ML pipeline to train an object detection model for recognizing political party logos in real-life videos."
    - title: "Tiktok scraper" 
      description: "Developed a data scraper for TikTok, leveraging audio transcription models and text processing to extract insights from short videos."
      link: "https://github.com/DaliaO15/Tiktok-scraping"
    - title: "Object detection workshop"
      description: "Led and designed a workshop on object detection with Roboflow and the YOLO family."
  2022:
    - title: "Project Delta"
      description: "A web development initiative."
      url: /project-delta/
  2020:
  2019:
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

## Past Projects and Participation

{% for year in page.past_projects %}
### {{ year[0] }}
{% for project in year[1] %}
- {% if project.link %} **[{{ project.title }}]({{ project.link }})** {% else %} **{{ project.title }}** {% endif %}: {{ project.description }}
{% endfor %}
{% endfor %}


