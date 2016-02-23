{% if include.page != null %}
{% assign post = include.page %}
{% else %}
{% assign post = page %}
{% endif %}
{% for image in post.images %}<!--
-->{% if include.image == null or include.image == image.name %}<!--
--><a href="{{ post.imgfolder }}/{{ image.name }}" data-sub-html="{{ image.text }}" class="single_img" ><!--
--><img src="{{ post.imgfolder }}/t_{{ image.name }}" data-sub-html="{{ image.text }}"></a><!--
-->{% endif %}{% endfor %}
