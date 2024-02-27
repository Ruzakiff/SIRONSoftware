   ---
   layout: default
   title: Changelog
   ---

   # Changelog

   {% for change in site.changelog %}
     <h2><a href="{{ change.url }}">{{ change.title }}</a></h2>
     <p>{{ change.date | date: "%B %d, %Y" }}</p>
     <p>{{ change.excerpt }}</p>
   {% endfor %}