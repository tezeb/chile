{% if include.page != null %}
{% assign post = include.page %}
{% else %}
{% assign post = page %}
{% endif %}
<div class="row">{% for image in post.images %}<!--
-->{% if include.image == null or include.image == image.name %}<!--
--><a href="{{ post.imgfolder }}/{{ image.name }}" data-lightbox="0" title="{{ image.text }}"><!--
--><img src="{{ post.imgfolder }}/{{ image.thumb }}" title="{{ image.text }}"></a><!--
-->{% endif %}{% endfor %}</div>
