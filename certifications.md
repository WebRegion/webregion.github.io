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
		        <div class="isotope-item col-12 col-lg-4 angular python-django">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="assets/images/projects/project-1-thumb.jpg" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-1-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="project.html">
								<h5 class="card-title font-weight-bold">Client: Google</h5>
							    <p class="card-text">Project summary goes here. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vel sapien quis nulla dictum euismod...</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="project.html">SaaS Product</a></h4>
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
		        
		        <div class="isotope-item col-12 col-lg-4 react">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="assets/images/projects/project-4-thumb.jpg" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-4-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="project.html">
								<h5 class="card-title font-weight-bold">Client: Dropbox</h5>
							    <p class="card-text">Project summary goes here. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vel sapien quis nulla dictum euismod...</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="project.html">Internal Product</a></h4>
						</div>
						
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">React</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">Flux</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">Babel</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">MongoDB</span></li>
							</ul>
					    </div>
				    </div><!--//card-->
		        </div><!--//isotope-item-->
		        
		        <div class="isotope-item col-12 col-lg-4 react php">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="assets/images/projects/project-5-thumb.jpg" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-5-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="project.html">
								<h5 class="card-title font-weight-bold">Client: Spotify</h5>
							    <p class="card-text">Project summary goes here. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vel sapien quis nulla dictum euismod...</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="project.html">Mobile App</a></h4>
						</div>
						
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">React</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">PHP</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">MySQL</span></li>
							</ul>
					    </div>
				    </div><!--//card-->
		        </div><!--//isotope-item-->
		        
		        <div class="isotope-item col-12 col-lg-4 ruby-rails">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="assets/images/projects/project-6-thumb.jpg" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-6-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="project.html">
								<h5 class="card-title font-weight-bold">Client: Evernote</h5>
							    <p class="card-text">Project summary goes here. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vel sapien quis nulla dictum euismod...</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="project.html">Web App &amp; Chrome Extension</a></h4>
						</div>
						
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">JavaScript</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">Ruby</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">HTML/CSS</span></li>
							</ul>
					    </div>
				    </div><!--//card-->
		        </div><!--//isotope-item-->
		        
		        <div class="isotope-item col-12 col-lg-4 angular php">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="assets/images/projects/project-7-thumb.jpg" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-7-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="project.html">
								<h5 class="card-title font-weight-bold">Client: Facebook</h5>
							    <p class="card-text">Project summary goes here. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vel sapien quis nulla dictum euismod...</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="project.html">Facebook Ads Manager</a></h4>
						</div>
						
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">Angular</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">PHP</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">HTML/SaSS</span></li>
							</ul>
					    </div>
				    </div><!--//card-->
		        </div><!--//isotope-item-->
		        
		        <div class="isotope-item col-12 col-lg-4 react python-django">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="assets/images/projects/project-8-thumb.jpg" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-8-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="project.html">
								<h5 class="card-title font-weight-bold">Client: Zendesk</h5>
							    <p class="card-text">Project summary goes here. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vel sapien quis nulla dictum euismod...</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="project.html">Mobile App Development</a></h4>
						</div>
						
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">React</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">Django</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">HTML/SaSS</span></li>
							</ul>
					    </div>
				    </div><!--//card-->
		        </div><!--//isotope-item-->
		        
		        
		        <div class="isotope-item col-12 col-lg-4 angular python-django">
					<div class="card rounded-0 border-0 shadow-sm mb-5">
						<div class="card-img-container position-relative">
							<img class="card-img-top rounded-0" src="assets/images/projects/project-9-thumb.jpg" alt="">
							<div class="card-img-overlay overlay-logo text-center">
								<div class="project-logo"><img class="img-fluid w-50" src="assets/images/logos/logo-9-inverse.svg"></div>
							</div>
							<a class="card-img-overlay overlay-content text-start p-lg-4" href="project.html">
								<h5 class="card-title font-weight-bold">Client: Coinbase</h5>
							    <p class="card-text">Project summary goes here. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vel sapien quis nulla dictum euismod...</p>
							</a>
						</div>
						<div class="card-body pb-0">
							<h4 class="card-title text-truncate text-center mb-0"><a class="text-link" href="project.html">App Development</a></h4>
						</div>
						
						<div class="card-footer border-0 text-center bg-white pb-4">
							<ul class="list-inline mb-0 mx-auto">
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">Angular</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">Python</span></li>
						        <li class="list-inline-item"><span class="badge bg-secondary badge-pill">HTML/SaSS</span></li>
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
        {% assign sertifications = site.sertifications | sort:"sertifications.date" | reverse %}
        {% for sertificate in sertifications %}
		    <div class="col-12 col-md-6 col-lg-4 mb-5">
			    <div class="card rounded-0 border-0 shadow-sm eq-height">
					<div class="card-img-container position-relative">
				        <img class="card-img-top rounded-0" src="assets/images/blog/blog-post-thumb-3.jpg" alt="">
				        <div class="card-img-overlay overlay-mask  text-center p-0">
					        <div class="overlay-mask-content text-center w-100 position-absolute">
							    <a class="btn btn-primary" href="{{ sertificate.url }}">Read more</a>
					        </div>
					        <a class="overlay-mask-link position-absolute w-100 h-100" href="{{ sertificate.url }}"></a>
						</div>
					</div>
					<div class="card-body pb-4">
						<h4 class="card-title mb-2"><a class="text-link" href="{{ sertificate.url }}">{{ sertificate.name }}</a></h4>
							<div class="card-text">
								<div class="excerpt">{{ sertificate.short-desc }}</div>
							</div>
						</div>
						<div class="card-footer border-0">
							<ul class="meta list-inline mb-0">
								<li class="list-inline-item me-3"><i class="far fa-clock me-2"></i>{{ sertificate.date | date: "%A, %d %b %Y" }}</li>
								<!--<li class="list-inline-item"><i class="fas fa-comment me-2"></i><a class="text-link" href="#">23 Comments</a></li>-->
							</ul>
						</div>
				    </div><!--//card-->
		        </div>
			{% endfor %}
		</div>
	</div>
</section>		
