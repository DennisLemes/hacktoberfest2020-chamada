---
---
# Chamada do Hacktoberfest 2020

{% for entry in site.data.chamada %}

<div style="display: inline-block; border: 1px solid gray; padding: 2px; width: 225px;">
<span><strong> {{ entry.nome }} </strong></span>
<br>
{% if entry.imagem %}
<img width=225 height=300 src="{{ site.baseurl }}/imgs/{{ entry.imagem }}">
{% else %}
<img width=225 height=300 src="https://cataas.com/cat/says/{{ entry.nome }} não tem foto">
{% endif %}
<br>
<span><small> {% include {{ entry.arquivo }} %} </small></span>
</div>

{% endfor %}