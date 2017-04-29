---
layout: page
permalink: /more/work_experience/
title: Work Experience
experiences:

    - title:   "Engineer III at WalmartLabs,Bangalore"
      time:    "October 2016 - Present"
      projects:
        -   name:  "Working on a project that deals with the 'Top 1 Million Items' in the world using various heuristic and data analysis techniques"
        -   name:  "Working on the architecture of the crawler component for the next generation CIA system"
        -   name:  "Worked on algorithms for matcher component of the CIA system."
      tags:    "Python, Java, Hadoop, Machine Learning"


    - title:   "MTS-II at Adobe Systems, Bangalore"
      time:    "August 2014 - May 2016"
      projects:
        -   name:  "Worked with the Creative Cloud Platform and Services team."
        -   name:  "Worked on Device SDK, an Android SDK for manipulating SVG images required by other mobile applications"
        -   name:  "Worked on Creative SDK which provides a rich set of components for a seamless workflow between mobile/desktop applications, Adobe tools and Creative Cloud Services."
      tags:    "Android, Java, C++"

---
{% assign thumbnail="left" %}

{% for pub in page.experiences %}
{% if pub.image %}
{% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
{% endif %}
{{pub.title}}<br />
{% if pub.projects %}<br />Project:<br/> {% for project in pub.projects %}{{project.name}}<br/>{% endfor %}{% endif %}
{% endfor %}
