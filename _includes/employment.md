<h2 id="publications" style="margin: 2px 0px -15px;">Employment</h2>

<div class="publications">

{% for link in site.data.experience.main %}
{% if link.type contains "job" %}
<div class="pub-row">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><b>{{ link.title }}</b></div>
      <div class="author">{{ link.institution }} {% if link.department %}| {{ link.department }} {% endif %}{% if link.years %}| {{ link.years }}{% endif %}</div>
  </div>{% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
</div><br>

{% endif %}
{% endfor %}
</div>