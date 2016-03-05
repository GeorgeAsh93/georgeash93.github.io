---
layout: intro
title: George Ash
---
{% include JB/setup %}

<ul>
  {% for post in site.posts %}
	<table style="width:100%">
	<tr>
	<td valign="bottom">
	<img src="{{site.url}}/images/{{post.site_image}}" align="left"/>
	</td>
	</tr>
	<tr>
	<td valign="top">
	<b><font size="4"><a href="{{ post.site_link }}">{{ post.title }}</a></font></b><br>
	</td>
	</tr>
	<tr>
	<td>
	<b>{{ post.date | date_to_string }}</b> 
	<a href="{{ post.site_link }}">{{ post.site_name }}</a> <br>
	</td>
	</tr>
	<tr>
	<td>
	{{ post.content | strip_html | truncatewords:40}}
            <a href="{{ post.site_link }}">Read more...</a><br><br><br><br>
	</td>
	</tr>
	</table>
  {% endfor %}
</ul>