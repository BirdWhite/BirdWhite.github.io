---
layout: default
permalink: /
---

<!-- Section -->
<section>
	<header class="major">
		<h2>목적</h2>
	</header>
	<div class="features">
	<article>
		<span class="icon solid fa-share-alt"></span>
		<div class="content">
			<h3>공유</h3>
			<p>지식을 공유함으로써 더 큰 가치를 창출하기 위해 노력합니다.</p>
		</div>
	</article>
		<article>
			<span class="icon fa-gem"></span>
			<div class="content">
				<h3>저장</h3>
				<p>지식을 저장하여 필요할 때 복기할 수 있도록 합니다.</p>
			</div>
		</article>
		<article>
			<span class="icon solid fa-universal-access"></span>
			<div class="content">
				<h3>접근성</h3>
				<p>개발 분야의 접근성을 향상해 누구나 개발할 수 있다는 말을 알리려 노력합니다.</p>
			</div>
		</article>

		<article>
			<span class="icon solid fa-gamepad"></span>
			<div class="content">
				<h3>흥미</h3>
				<p>본 블로그는 저자의 흥미에 기반하여 포스팅됩니다.</p>
			</div>
		</article>
	</div>
</section>

<section>
  <ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
  </ul>
</section>
