## Publications

{% for paper in site.data.publications.main %}
1. {% if paper.link %}<a href="{{ paper.link }}"><papertitle>{{ paper.title }}</papertitle></a>{% else %}<papertitle>{{ paper.title }}</papertitle>{% endif %}

   {{ paper.authors }}

   {{ paper.conference }}

   {% if paper.pdf %}<a href="{{ paper.pdf }}">PDF</a>{% endif %}
   {% if paper.code %}<a href="{{ paper.code }}">Code</a>{% endif %}
   {% if paper.page %}<a href="{{ paper.page }}">Project Page</a>{% endif %}
   {% if paper.notes %}{{ paper.notes }}{% endif %}
{% endfor %}
