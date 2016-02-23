<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <title>{% if page.title %}{{ page.title }}{% else %}{{ site.title }}{% endif %}</title>
  <meta name="description" content="{% if page.excerpt %}{{ page.excerpt | strip_html | strip_newlines | truncate: 160 }}{% else %}{{ site.description }}{% endif %}">

  <link rel="stylesheet" href="{{ "/css/main.css" | prepend: site.baseurl }}">
  <script src="/js/jquery-1.10.2.min.js"></script>
  <script src="/js/lightgallery.min.js"></script>
  <link href="/css/lightgallery.min.css" rel="stylesheet" />
  <link rel="canonical" href="{{ page.url | replace:'index.html','' | prepend: site.baseurl | prepend: site.url }}">
  <link href='http://fonts.googleapis.com/css?family=Open+Sans:400,300,600,700' rel='stylesheet' type='text/css'>
</head>
