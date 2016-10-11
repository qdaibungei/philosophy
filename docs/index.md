---
layout: index
---

<div id="PAGETOP">


<!--================-->
<!--　　ヘッダー　　-->
<!--================-->
<div id="HEADER">
<h1>九州大学文藝部・哲学会</h1>
	<ul id="PAN">
		<li>HOME</li>
	</ul>
</div>
<hr>


<!--================-->
<!--　　メニュー　　-->
<!--================-->
<div id="MENU">
<h2>menu</h2>
	<ul>
		<li id="MENU01" class="menu-on"><a href="{{ site.baseurl }}">HOME</a></li>
		<li id="MENU02"><a href="{{ site.baseurl }}/about/">ABOUT</a></li>
		<li id="MENU03"><a href="{{ site.baseurl }}/documents/">DOCUMENTS</a></li>
	</ul>
</div>
<hr>


<!--================-->
<!--　　記事部分　　-->
<!--================-->
<div id="KIZI">


<div class="text">

{% for post in site.posts limit:1 %}
<h2>{{ post.title }}</h2>
<p>（以下、最新記事）</p>
{{ post.content }}
{% endfor %}



<ul class="modori">
  <li><a href="#PAGETOP">TOP</a></li>
</ul>
</div>
<hr>



<h2>Recent Documents</h2>
<div class="text">
<ul>
{% for post in site.posts limit:5 %}
  <li>
    <a href="{{ site.baseurl }}{{ post.url }}"><code>{{ post.date | date: "%Y-%m-%d" }}</code>　{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

<ul class="modori">
  <li><a href="#PAGETOP">TOP</a></li>
</ul>
</div>
<hr>




</div>


<!--================-->
<!--　　フッター　　-->
<!--================-->
<div id="FOOTER">
<h2>連絡先</h2>
	<ul>
		<li id="FOOTER01">©2016 哲学会</li>
	</ul>
</div>


</div>
