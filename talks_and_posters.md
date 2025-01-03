---
layout: default
---

# Talks

{% for info in site.data.talks %}

<div class="talk-info">
<h3>{{ info.event }}<span> — {{ info.location }} ({{ info.date }})</span></h3>
{{ info.title }}
{% if info.pdf %}
[<a href="{{ site.url }}/assets/pdfs/talks/{{ info.pdf }}" target="_blank">slides</a>]
{% endif %}
</div>

{% endfor %}

# Posters

{% for info in site.data.posters %}

<div class="poster-info">
<h3>{{ info.event }}<span> — {{ info.location }} ({{ info.date }})</span></h3>
{% if info.pdf %}
<a href="{{ site.url }}/assets/pdfs/posters/{{ info.pdf }}" target="_blank">
{% endif %}
{{ info.title }}
{% if info.pdf %}
</a>
{% endif %}
</div>

{% endfor %}
