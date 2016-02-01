		<a title="{{ include.title_prefix }}{{include.post.title}}" href="{{ include.post.url }}">
			{{ include.prefix }}
			<!-- Whitespace added for readability -->
			{% assign d = include.post.date | date: "%-d"  %}
			{{ include.post.date | date: "%B" }} 
			{% case d %}
			{% when '1' or '21' or '31' %}{{ d }}st,
			{% when '2' or '22' %}{{ d }}nd,
			{% when '3' or '23' %}{{ d }}rd,
			{% else %}{{d}}th,
			{% endcase %}
			{{ include.post.date | date: "%Y" }} - {{ include.post.title }}
			{{ include.suffix }}
			</a>
