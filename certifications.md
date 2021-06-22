---
layout: default
title: Мои сертификаты
---
<section class="section pt-5">
    <div class="container">
	        <div class="text-center">
		        <ul id="filters" class="filters mb-5 mx-auto ps-0">
					<li class="type active" data-filter="*">All</li>
{% assign rawtags = "" %}
{% for certifications2 in site.certifications %}
	{% assign ttags = certifications2.tags | join:'|' | append:'|' %}
	{% assign rawtags = rawtags | append:ttags %}
{% endfor %}
{% assign rawtags = rawtags | split:'|' | sort %}
{% assign tags = "" %}
{% for tag in rawtags %}
	{% if tag != "" %}
		{% if tags == "" %}
			{% assign tags = tag | split:'|' %}
		{% endif %}
		{% unless tags contains tag %}
			{% assign tags = tags | join:'|' | append:'|' | append:tag | split:'|' %}
		{% endunless %}
	{% endif %}
{% endfor %}
{% for tag in tags %}
	<li class="type" data-filter=".{{ tag }}">{{ tag | capitalize }}</li>
{% endfor %}
	            </ul><!--//filters-->
	        </div>
		
			
			
			<div class="project-cards row mb-5 isotope">			
    {% assign certifications1 = site.certifications | sort: 'date' %}
	
    {% for certificate in certifications1 %}		
		        <div class="isotope-item col-12 col-lg-4 angular python-django">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="/images/certificates/{{ certificate.image-name }}" alt="">
							<!--<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-1-inverse.svg"></div>
							</div>-->
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="{{ certificate.url }}">
								<h5 class="card-title font-weight-bold">{{ certificate.name }}</h5>
							    <p class="card-text">{{ certificate.short-desc }}</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="{{ certificate.url }}">{{ certificate.name }}</a></h4>
						</div>
						{% if certificate.tags %}
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
								{% for tag in certificate.tags %}
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">{{ tag | capitalize }}</span></li>
								{% endfor %}
							</ul>
					    </div>
						{% endif %}
				    </div><!--//card-->
		        </div><!--//isotope-item-->
	{% endfor %}
	
		        
		        <div class="isotope-item col-12 col-lg-4 ruby-rails">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="assets/images/projects/project-2-thumb.jpg" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-2-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="project.html">
								<h5 class="card-title font-weight-bold">Client: Basecamp</h5>
							    <p class="card-text">Project summary goes here. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vel sapien quis nulla dictum euismod...</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="project.html">Webapp Development</a></h4>
						</div>
						
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill" >Rails</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">jQuery</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">PostgresSQL</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">HTML/LESS</span></li>
							</ul>
					    </div>
				    </div><!--//card-->
		        </div><!--//isotope-item-->
		        
		        <div class="isotope-item col-12 col-lg-4 react python-django">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="assets/images/projects/project-3-thumb.jpg" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-3-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="project.html">
								<h5 class="card-title font-weight-bold">Client: Airbnb</h5>
							    <p class="card-text">Project summary goes here. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vel sapien quis nulla dictum euismod...</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="project.html">Mobile app development</a></h4>
						</div>
						
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">React</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill" >Python</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">MySQL</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">Webpack</span></li>
							</ul>
					    </div>
				    </div><!--//card-->
		        </div><!--//isotope-item-->
		        

		        

			    
	        </div><!--//row-->

        </div><!--//container-->
    </section><!--//section-->



































<section class="section pt-5">
    <div class="container blog-cards">	        
	    <div class="row">
        {% assign certifications = site.certifications | sort: 'date' %}
        {% for certificate in certifications %}
		    <div class="col-12 col-md-6 col-lg-4 mb-5">
			    <div class="card rounded-0 border-0 shadow-sm eq-height">
					<div class="card-img-container position-relative">
				        <img class="card-img-top rounded-0" src="assets/images/blog/blog-post-thumb-3.jpg" alt="">
				        <div class="card-img-overlay overlay-mask  text-center p-0">
					        <div class="overlay-mask-content text-center w-100 position-absolute">
							    <a class="btn btn-primary" href="{{ certificate.url }}">Read more</a>
					        </div>
					        <a class="overlay-mask-link position-absolute w-100 h-100" href="{{ certificate.url }}"></a>
						</div>
					</div>
					<div class="card-body pb-4">
						<h4 class="card-title mb-2"><a class="text-link" href="{{ certificate.url }}">{{ certificate.name }}</a></h4>
							<div class="card-text">
								<div class="excerpt">{{ certificate.short-desc }}</div>
							</div>
						</div>
						<div class="card-footer border-0">
							<ul class="meta list-inline mb-0">
								<li class="list-inline-item me-3"><i class="far fa-clock me-2"></i>{{ certificate.date | date: "%A, %d %b %Y" }}</li>
								<!--<li class="list-inline-item"><i class="fas fa-comment me-2"></i><a class="text-link" href="#">23 Comments</a></li>-->
							</ul>
						</div>
				    </div><!--//card-->
		        </div>
			{% endfor %}
		</div>
	</div>
</section>		
