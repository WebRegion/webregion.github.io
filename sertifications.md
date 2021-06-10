---
layout: default
title: Мои сертификаты
---
<section class="section pt-5">
    <div class="container blog-cards">	        
	    <div class="row">
        {% assign sertifications = site.sertifications | sort: 'date' %}
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
