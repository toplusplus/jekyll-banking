---
title: About Us
subtitle: Sed tincidunt lorem
description:
- chunk: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tincidunt lorem
    sed velit fermentum lobortis, eget placerat mauris sed lectus tellus.
- chunk: Fusce eu semper lacus, sodales id elit a, feugiat porttitor nulla. Sed porta
    magna vitae nisl vulputate lacinia.
features:
- name: Duis aute irure dolor in reprehenderit voluptate
- name: Excepteur sint occaecat cupidatat non proident
- name: Sunt in culpa qui officia deserunt mollit
- name: Duis aute irure dolor in reprehenderit voluptate
- name: Excepteur sint occaecat cupidatat non proident
---

	<!-- about -->
	<div class="about" id="about">
		<div class="container">
			<div class="w3-welcome-heading">
				<h3>{{ site.data.about.title }}</h3>
			</div>
			<div class="w3ls-about-grids">
				<div class="col-md-6 about-right">
					<img src="{{site.baseurl}}/assets/images/9.jpg" alt="">
				</div>
				<div class="col-md-6 about-left"> 
					<h4>{{ site.data.about.subtitle }}</h4>

					{% for item in site.data.about.description %}
					<p>{{ item.chunk }}</p>
					{% endfor %}						

					<ul> 
						{% for item in site.data.about.features %}
						<li><span class="glyphicon glyphicon-share-alt"></span> {{ item.name }}</li>
						{% endfor %}						
					</ul>
				</div>
				<div class="clearfix"> </div>
			</div>
		</div>
	</div>
	<!-- //about -->