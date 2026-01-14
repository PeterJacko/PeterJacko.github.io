---
layout: archive
title: "Expertise Hub"
permalink: /
author_profile: true
---

Welcome to my professional hub. I offer high-level **consultancy, research collaboration, and specialist training** at the intersection of Statistics, Operational Research, and Machine Learning. With over two decades of experience across academia and the pharmaceutical industry, I provide expertise in:

* **Clinical Trials:** Designing efficient, patient-centric adaptive and platform trials.
* **Resource Allocation:** Optimizing dynamic systems through restless bandits and index policies.
* **Teaching & Mentoring:** Delivering bespoke professional training and high-impact research supervision.
* **Strategic Leadership:** Proven track record in coordinating international research groups and mathematical science networks, with extensive evidence of service available on my [CV page](/cv/).

---

# 📢 Latest Updates & Insights

{% for post in site.posts limit:10 %}
  <article style="margin-bottom: 3em; border-bottom: 1px solid #eee; padding-bottom: 2em;">
    
    {% if post.tags contains "news" %}
      <h3 style="margin-bottom: 0.2em; color: #333;">{{ post.title }}</h3>
      <small style="color: #666;">{{ post.date | date: "%B %d, %Y" }} • <strong>News</strong></small>
      
      <div style="margin-top: 1em; line-height: 1.6;">
        {{ post.content }}
      </div>

      <div style="margin-top: 1.5em; font-size: 0.85em; background: #f9f9f9; padding: 10px; border-radius: 4px;">
        <strong style="margin-right: 10px;">Share update:</strong>
        <a href="https://www.linkedin.com/sharing/share-offsite/?url={{ site.url }}{{ post.url }}" target="_blank" style="margin-right: 12px;">LinkedIn</a>
        <a href="https://x.com/intent/post?text={{ post.title | url_encode }}&url={{ site.url }}{{ post.url }}" target="_blank" style="margin-right: 12px;">X</a>
        <a href="https://api.whatsapp.com/send?text={{ post.title | url_encode }}%20{{ site.url }}{{ post.url }}" target="_blank" style="margin-right: 12px;">WhatsApp</a>
        <a href="mailto:?subject={{ post.title | url_encode }}&body={{ site.url }}{{ post.url }}">Email</a>
      </div>

    {% else %}
      <h3 style="margin-bottom: 0.2em;"><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></h3>
      <small style="color: #666;">{{ post.date | date: "%B %d, %Y" }} • <strong>Blog Post</strong></small>
      
      <div style="margin-top: 0.8em;">
        {{ post.excerpt | strip_html | truncatewords: 60 }}
      </div>
      
      <div style="margin-top: 1em;">
        <a href="{{ base_path }}{{ post.url }}" style="font-weight: bold;">Read full article →</a>
      </div>
    {% endif %}

  </article>
{% endfor %}

---

# 📢 Latest News & Insights

{% for post in site.posts limit:5 %}
  <article style="margin-bottom: 2.5em; border-bottom: 1px solid #eee; padding-bottom: 1.5em;">
    <h3 style="margin-bottom: 0.2em;"><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></h3>
    <small style="color: #666;">{{ post.date | date: "%B %d, %Y" }}</small>
    
    <div style="margin-top: 0.8em;">
      {{ post.excerpt | strip_html | truncatewords: 50 }}
    </div>

    <div style="margin-top: 1.2em; font-size: 0.85em; color: #444;">
      <strong>Share:</strong>
      <a href="https://www.linkedin.com/sharing/share-offsite/?url={{ site.url }}{{ post.url }}" target="_blank" style="margin-right: 10px;">LinkedIn</a>
      <a href="https://twitter.com/intent/tweet?text={{ post.title | url_encode }}&url={{ site.url }}{{ post.url }}" target="_blank" style="margin-right: 10px;">X</a>
      <a href="https://api.whatsapp.com/send?text={{ post.title | url_encode }}%20{{ site.url }}{{ post.url }}" target="_blank" style="margin-right: 10px;">WhatsApp</a>
      <a href="mailto:?subject={{ post.title | url_encode }}&body=Check out this update from Peter Jacko: {{ site.url }}{{ post.url }}" style="margin-right: 10px;">Email</a>
    </div>
  </article>
{% endfor %}

[View Full Archive](/posts/)
---

## 📬 Stay Connected
* **RSS Feed:** Subscribe via [RSS Feed]({{ base_path }}/feed.xml) for automatic updates.
* **LinkedIn:** Connect for professional updates on [LinkedIn](https://www.linkedin.com/in/peterjacko/).
