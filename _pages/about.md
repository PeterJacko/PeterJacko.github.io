---
layout: archive
title: "Peter Jacko"
permalink: /
author_profile: true
---

I am a Senior Lecturer in the Department of Management Science at **Lancaster University**, and a Senior Decision Scientist at **Berry Consultants**. My work sits at the intersection of **Statistics, Operational Research, and Machine Learning**. 

My research focuses on the design and analysis of optimal priority rules for dynamic systems, with a particular emphasis on:
* **Clinical Trials:** Developing adaptive and patient-centric designs.
* **Resource Allocation:** Whittle index policies and restless bandits.

---

# 📢 Recent News

{% for post in site.posts limit:5 %}
  <article style="margin-bottom: 2em; border-bottom: 1px solid #eee; padding-bottom: 1em;">
    <h3 style="margin-bottom: 0.2em;"><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></h3>
    <small style="color: #666;">{{ post.date | date: "%B %d, %Y" }}</small>
    
    <div style="margin-top: 0.5em;">
      {{ post.excerpt | strip_html | truncatewords: 50 }}
    </div>

    <div style="margin-top: 1em; font-size: 0.9em;">
      <a href="{{ base_path }}{{ post.url }}">Read More</a> | 
      <a href="https://www.linkedin.com/sharing/share-offsite/?url={{ site.url }}{{ post.url }}" target="_blank">Share on LinkedIn</a> |
      <a href="https://twitter.com/intent/tweet?text={{ post.title }}&url={{ site.url }}{{ post.url }}" target="_blank">Share on X</a>
    </div>
  </article>
{% endfor %}

[See all news](/posts/)

---

## 📬 Stay Connected
* **RSS Feed:** Subscribe via [RSS Feed]({{ base_path }}/feed.xml) for automatic updates.
* **LinkedIn:** Connect for professional updates on [LinkedIn](https://www.linkedin.com/in/peterjacko/).
