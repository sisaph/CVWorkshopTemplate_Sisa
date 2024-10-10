<h2 id="publications" style="margin: 2px 0px -15px;">Employment</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.experience.main %}
{% if link.type contains "job" %}

<div class="pub-row">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">{{ link.title }}</div>
      <div class="author">{{ link.institution }} | {{ link.department }} | {{ link.years }}</div>
  </div>
</div>

{% endif %}
{% endfor %}
</ol>
</div>