---
layout: default
title: Мои сертификаты
---
    <section class="section pt-5">
        <div class="container">
	        <div class="text-center">
		        <ul id="filters" class="filters mb-5 mx-auto ps-0">
	                <li class="type active" data-filter="*">All</li>
	                <li class="type" data-filter=".angular">Angular</li>
	                <li class="type" data-filter=".react">React</li>
	                <li class="type" data-filter=".python-django">Python/Django</li>
	                <li class="type" data-filter=".ruby-rails">Ruby/Rails</li>
	                <li class="type" data-filter=".php">PHP</li>
	            </ul><!--//filters-->
	        </div>
	        <div class="project-cards row mb-5 isotope">
        {% assign certifications = site.certifications | sort:"certifications.date" | reverse %}
        {% for certificate in certifications %}			
		        <div class="isotope-item col-12 col-lg-4 angular python-django">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="{{ certificate.image-cert }}" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-1-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="{{ certificate.url }}">
								<h5 class="card-title font-weight-bold">{{ certificate.title }}</h5>
							    <p class="card-text">{{ certificate.short-desc }}</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="{{ sertificate.url }}">SaaS Product</a></h4>
						</div>
						
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">Angular</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill" >Django</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">MongoDB</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">HTML/CSS</span></li>
							</ul>
					    </div>
				    </div><!--//card-->
		        </div><!--//isotope-item-->
			{% endfor %}				
	        </div><!--//row-->

        </div><!--//container-->
    </section><!--//section-->
	