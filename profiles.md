---
layout: page
title: Profiles
permalink: /more/profiles/
profs:
      - name: "HackerRank"
        url:    "https://www.hackerrank.com/shan8913"
        image:  "../../images/hackerrank.jpg"

      - name: "LeetCode"
        url:	"https://leetcode.com/shan892015/"
        image:	"../../images/leetCode.png" 
      
      - name: "Kaggle"
        url:	""
        image:	"../../images/kaggle.png"

      - name: "Linkedin"
        url:	"https://www.linkedin.com/in/shankarlalagarwal/"
        image:	"../../images/linkedin.jpg"       
---
<!-- profiles:

	- name: 	"HackerRank"
	  url:		"https://www.hackerrank.com/shan8913"
	  image:	"images/hackerrank.jpg"

-->
You can check out my various profiles......

{% assign thumbnail="left" %}
{% for pub in page.profs %}
{% if pub.image %}
{% include image.html url=pub.image caption="" all="" height="25px" width="50px" align=thumbnail %}
{% endif %}
[**{{pub.name}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{% endfor %}