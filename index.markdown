---
layout: default
---

{% include button-style.html %}

[Download Extension](/assets/files/SIRONECMS.zip){: .download-button}

{% include stripe_button.html %}
{% include rebind_form.html %}

{% include gif_timer.html baseurl=site.baseurl %}

## Recent Updates

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | absolute_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}