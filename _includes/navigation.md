{% if page.lang == 'zh' %}{% assign navlinks = site.data.navigation.zh %}{% else %}{% assign navlinks = site.data.navigation.main %}{% endif %}
{% if page.alt_lang_url %}
<a class="normal right lang-switch" href="{{ page.alt_lang_url }}">{% if page.lang == 'zh' %}English{% else %}中文{% endif %}</a>
{% endif %}
{% for link in navlinks %}
<a class="normal" href="{{ link.url }}">{{ link.title }}</a>
{% endfor %}
