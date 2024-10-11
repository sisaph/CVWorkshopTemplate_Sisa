<h2 id="publications" style="margin: 2px 0px -15px;">Awards</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.pubscombined.main %}
{% if link.type contains "award" %}



  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><b>{{ link.title }}</b> | {{ link.institution }}{% if link.amount %} | {{ link.amount }}{% endif %} | {{ link.date }}</div>
      {% if link.awardedfor %}<div class="author" style="position: relative;padding-left: 10px;">Awarded for: {{ link.awardedfor }}{% endif %}
      </div>
    <div class="links">
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
    </div>
  </div>
{% endif %}
{% endfor %}

</ol>
</div>

