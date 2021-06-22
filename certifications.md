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
			    
	        </div><!--//row-->

        </div><!--//container-->
    </section><!--//section-->
