---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: wrapper
extra_css: introduction.css
---

<section id="intro-section" class="auto-height">
	<div id="intro-content">
		<h2>Hi!</h2>
		<p>
			I'm William Adams and I like making and playing games. 
			I like all kinds of games, but my favorites are definitely strategy and competitive games.<br/> 
			Here you can find some of the games and other projects I've made. Feel free to contact me by email or LinkedIn <a href="/contact">here</a>.
		</p>
	</div>
	<img src="/assets/pictures/portrait.jpg" id="portrait" alt="Portrait">
</section>

<section>
	{% include project_list.html type=site.data.project-types.solo-games %}
</section>

<section>
	{% include project_list.html type=site.data.project-types.other %}
</section>