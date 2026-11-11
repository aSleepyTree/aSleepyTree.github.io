## Publications

<style>
.publications {
  margin-top: 4px;
}

.publication-list {
  list-style: none;
  margin: 0;
  padding: 0;
}

.publication-list li {
  margin-bottom: 22px;
}

.pub-row {
  display: flex;
  gap: 16px;
  align-items: flex-start;
}

.pub-media {
  flex: 0 0 230px;
  position: relative;
}

.pub-media img {
  background: #fff;
  border: 1px solid #e6e6e6;
  border-radius: 6px;
  box-sizing: border-box;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.10);
  display: block;
  height: 128px;
  object-fit: contain;
  width: 230px;
}

.pub-badge {
  background: #043361;
  border-radius: 4px;
  color: #fff;
  font-size: 11px;
  font-weight: 600;
  left: 7px;
  line-height: 1;
  padding: 4px 7px;
  position: absolute;
  top: 7px;
}

.pub-content {
  flex: 1;
  min-width: 0;
}

.pub-title {
  margin-bottom: 4px;
}

.pub-authors,
.pub-venue,
.pub-links {
  margin-bottom: 4px;
}

.pub-links a {
  border: 1px solid #bbb;
  border-radius: 4px;
  display: inline-block;
  font-size: 12px;
  margin: 2px 6px 2px 0;
  padding: 1px 7px;
}

@media print, screen and (max-width: 640px) {
  .pub-row {
    display: block;
  }

  .pub-media {
    margin-bottom: 9px;
  }

  .pub-media img {
    height: auto;
    max-height: 180px;
    width: 100%;
  }
}

@media (prefers-color-scheme: dark) {
  .pub-media img {
    border-color: #40414a;
  }

  .pub-links a {
    border-color: #6b6d78;
  }
}
</style>

<div class="publications">
<ol class="publication-list">
{% for paper in site.data.publications.main %}
  <li>
    <div class="pub-row">
      {% if paper.image %}
      <div class="pub-media">
        <img src="{{ paper.image | relative_url }}" alt="{{ paper.title }} teaser">
        {% if paper.badge %}<span class="pub-badge">{{ paper.badge }}</span>{% endif %}
      </div>
      {% endif %}
      <div class="pub-content">
        <div class="pub-title">
          {% assign title_link = paper.link | default: paper.pdf %}
          {% if title_link %}<a href="{{ title_link }}" target="_blank" rel="noopener"><papertitle>{{ paper.title }}</papertitle></a>{% else %}<papertitle>{{ paper.title }}</papertitle>{% endif %}
        </div>
        <div class="pub-authors">{{ paper.authors }}</div>
        <div class="pub-venue">{{ paper.conference }}</div>
        <div class="pub-links">
          {% if paper.link %}<a href="{{ paper.link }}" target="_blank" rel="noopener">Paper</a>{% endif %}
          {% if paper.pdf %}<a href="{{ paper.pdf }}" target="_blank" rel="noopener">PDF</a>{% endif %}
          {% if paper.code %}<a href="{{ paper.code }}" target="_blank" rel="noopener">Code</a>{% endif %}
          {% if paper.conference_url %}<a href="{{ paper.conference_url }}" target="_blank" rel="noopener">Conference</a>{% endif %}
          {% if paper.page %}<a href="{{ paper.page }}" target="_blank" rel="noopener">Project Page</a>{% endif %}
          {% if paper.notes %}{{ paper.notes }}{% endif %}
        </div>
      </div>
    </div>
  </li>
{% endfor %}
</ol>
</div>
