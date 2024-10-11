<h2 id="publications" style="margin: 2px 0px -15px;">Service</h2>

<div class="publications">
<ol class="bibliography">
{% for link in site.data.experience.main %}
{% if link.type contains "service" %}
<li>
<div class="pub-row">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">{{ link.title }}</div>
      <div class="author">{% if link.institution %}{{ link.institution }} {% endif %}{% if link.years %}{{ link.years }}{% endif %}</div></div></div></li>
{% endif %}
{% endfor %}
</ol>
</div>