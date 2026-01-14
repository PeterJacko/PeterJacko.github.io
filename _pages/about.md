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
      <h3 style="margin-bottom: 0.2em;">News: {{ post.title }}</h3>
      <small style="color: #666;">{{ post.date | date: "%Y %B %d" }}</small>
      
      <div style="margin-top: 0.8em;">
        {{ post.content }}
      </div>

      <!-- BEGIN copied from social_share.html REPLACING page.title BY post.title -->

      {% include base_path %}

      <section class="page__share">
      <!--  {% if site.data.ui-text[site.locale].share_on_label %}
          <h4 class="page__share-title">{{ site.data.ui-text[site.locale].share_on_label | default: "Share on" }}</h4>
        {% endif %} -->

        <button onclick="copyToClipboard()" class="btn btn--light" title="Copy Link to Clipboard" style="cursor: pointer;"><i class="fas fa-fw fa-link" aria-hidden="true"></i><span> Link &nbsp;</span></button>

        <a href="mailto:?subject={{ post.title | url_encode }}&body=Check out this post from Peter Jacko: {{ base_path }}{{ page.url | url_encode }}" class="btn btn--mail" title="{{ site.data.ui-text[site.locale].share_on_label | default: 'Share on' }} Email" style="background-color: #777; border-color: #777;"><i class="fas fa-fw fa-envelope" aria-hidden="true"></i><span> Email</span></a>

        <a href="https://api.whatsapp.com/send?text={{ post.title | url_encode }}%20{{ base_path }}{{ page.url | url_encode }}" class="btn btn--success" title="{{ site.data.ui-text[site.locale].share_on_label | default: 'Share on' }} WhatsApp" style="background-color: #25D366; border-color: #25D366;"><i class="fab fa-fw fa-whatsapp" aria-hidden="true"></i><span> WhatsApp</span></a>

        <a href="https://www.linkedin.com/sharing/share-offsite/?url={{ base_path }}{{ page.url | url_encode }}" class="btn btn--linkedin" title="{{ site.data.ui-text[site.locale].share_on_label | default: 'Share on' }} LinkedIn"><i class="fab fa-fw fa-linkedin" aria-hidden="true"></i><span> LinkedIn</span></a>

        <a href="https://bsky.app/intent/compose?text={{ post.title | url_encode }}%20{{ base_path }}{{ page.url | url_encode }}" class="btn btn--bluesky" title="{{ site.data.ui-text[site.locale].share_on_label | default: 'Share on' }} Bluesky"><i class="fab fa-fw fa-bluesky" aria-hidden="true"></i><span> Bluesky</span></a>

        <a href="https://x.com/intent/post?text={{ post.title | url_encode }}%20{{ base_path }}{{ page.url | url_encode }}" class="btn btn--x" title="{{ site.data.ui-text[site.locale].share_on_label | default: 'Share on' }} X"><i class="fab fa-fw fa-x-twitter" aria-hidden="true"></i><span> X</span></a>

        <a href="https://www.facebook.com/sharer/sharer.php?u={{ base_path }}{{ page.url | url_encode }}" class="btn btn--facebook" title="{{ site.data.ui-text[site.locale].share_on_label | default: 'Share on' }} Facebook"><i class="fab fa-fw fa-facebook" aria-hidden="true"></i><span> Facebook</span></a>

        <a href="https://www.addtoany.com/add_to/mastodon?linkurl={{ base_path | append: page.url | url_encode }}" class="btn btn--mastodon" title="{{ site.data.ui-text[site.locale].share_on_label | default: 'Share on' }} Mastodon"><i class="fab fa-fw fa-mastodon" aria-hidden="true"></i><span> Mastodon</span></a>
      </section>

      <script>
      function copyToClipboard() {
        const url = "{{ base_path }}{{ page.url }}";
        navigator.clipboard.writeText(url).then(() => {
          // Simple feedback for the user
          const btn = event.currentTarget;
          const originalText = btn.innerHTML;
          btn.innerHTML = '<i class="fas fa-fw fa-check"></i><span> Copied!</span>';
          setTimeout(() => { btn.innerHTML = originalText; }, 2000);
        });
      }
      </script>

      <!-- END copied from social_share.html -->
      
      <div style="margin-top: 1.5em; font-size: 0.85em; background: #f9f9f9; padding: 10px; border-radius: 4px;">
        <strong style="margin-right: 10px;">Share update:</strong>
        <a href="https://www.linkedin.com/sharing/share-offsite/?url={{ site.url }}{{ post.url }}" target="_blank" style="margin-right: 12px;">LinkedIn</a>
        <a href="https://x.com/intent/post?text={{ post.title | url_encode }}&url={{ site.url }}{{ post.url }}" target="_blank" style="margin-right: 12px;">X</a>
        <a href="https://api.whatsapp.com/send?text={{ post.title | url_encode }}%20{{ site.url }}{{ post.url }}" target="_blank" style="margin-right: 12px;">WhatsApp</a>
        <a href="mailto:?subject={{ post.title | url_encode }}&body={{ site.url }}{{ post.url }}">Email</a>
      </div>

    {% else %}
      <h3 style="margin-bottom: 0.2em;"><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></h3>
      <small style="color: #666;">{{ post.date | date: "%Y %B %d" }}</small>
      
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
