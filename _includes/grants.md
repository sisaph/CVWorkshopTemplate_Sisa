<h2 id="publications" style="margin: 2px 0px -15px;">Fellowships and Grants</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.pubscombined.main %}
{% if link.type contains "grant" %}


  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <strong>{{ link.title }}</strong>{% if link.institution %} | {{ link.institution }}{% endif %}{% if link.amount %} | {{ link.date }}<br><b>{{ link.amount }}</b>{% endif %}
<div class="links">{% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}</div>
</div>

<br>

{% endif %}
{% endfor %}

</ol>
</div>

