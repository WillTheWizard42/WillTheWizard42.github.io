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
			I'm William Adams and I like coding and mathematics. <br/>
			I graduated from Grenoble INP - ENSIMAG, the most prestigious software engineering school in France, in September 2023. <br/><br/>
			I especially like making simulations and games, but also enjoy making other things.
			I like all kinds of games, but my favorites are definitely strategy and competitive games.<br/><br/>
			As a professional, I worked for two years on Microsoft Flight Simulator 2024. This allowed me to greatly improve many of my skills, particularly C++ programming.<br/><br/>
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