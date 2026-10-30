<h2 id="publications" class="pub-section-title" >论文发表</h2>

{% if site.data.preprints.main.size > 0 %}
<h3 class="pub-subsection" style="margin: 30px 0px -30px;">预印本</h3>


<div class="publications">
<ol class="bibliography">

{% for link in site.data.preprints.main %}

<li>
<div class="pub-row">
  {% if link.image %}
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1">
  </div>
  {% endif %}
  <div class="{% if link.image %}col-sm-9{% else %}col-sm-12{% endif %}" style="position: relative;padding-right: 15px;padding-left: {% if link.image %}20px{% else %}15px{% endif %};">
      <div class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">代码</a>
      {% endif %}
      {% if link.notes %} 
      <i style="color:#e74d3c;">{{ link.notes_zh | default: link.notes }}</i>
      {% endif %}
    </div>
  </div>
</div>
</li>


{% endfor %}

</ol>
</div>

<h3 class="pub-subsection" style="margin: 35px 0px -30px;">正式发表</h3>
{% endif %}


<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  {% if link.image %}
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1">
  </div>
  {% endif %}
  <div class="{% if link.image %}col-sm-9{% else %}col-sm-12{% endif %}" style="position: relative;padding-right: 15px;padding-left: {% if link.image %}20px{% else %}15px{% endif %};">
      <div class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</div>
      <div class="author">{{ link.authors_zh | default: link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">代码</a>
      {% endif %}
      {% if link.notes %} 
      <i style="color:#e74d3c;">{{ link.notes_zh | default: link.notes }}</i>
      {% endif %}
    </div>
  </div>
</div>
</li>

{% endfor %}

</ol>
</div>
