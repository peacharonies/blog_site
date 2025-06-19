---
layout: default
title: Home
---


<!DOCTYPE html>
<html lang='en'>

<head>
	<meta charset='UTF-8'>
	<meta name='viewport' content='width=device-width, initial-scale=1' user-scalable='yes'>
	<title>Peacharonies: Blog</title>
	<style>
		body {padding: 0px 30px}
		ul {list-style-type: none;}
		li {white-space: pre-line;
			font-size: 25px;}
		h1 {margin-bottom: 0px;}		
		h2 {margin-top: 0px;
			font-size: 20px;
			opacity: 60%;}
	</style>
</head>

<body>
	<h1>Peacharonies
		<h2>The Peachy Observer</h2>
	</h1>
	<hr />
	<a href='https://www.peacharonies.com'>Home</a> | <a href='https://blog.peacharonies.com'>Blog</a>
	<hr />
	<br />
	{% for post in site.posts %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt }}</p>
{% endfor %}
	

</body>

</html>
