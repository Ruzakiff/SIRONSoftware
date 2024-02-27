---
layout: default
---

{% include button-style.html %}

[Download Extension](/assets/files/SIRONECMS.zip){: .download-button}

{% include stripe_button.html %}
{% include rebind_form.html %}

{% include gif_timer.html baseurl=site.baseurl %}

## Recent Updates

{% for change in site.changelog limit:5 %}
- [{{ change.title }}]({{ change.url }}) - {{ change.date | date: "%B %d, %Y" }}
{% endfor %}