# Portfolio-website
<!DOCTYPE html>
<html lang="en">

<head>
	<title>Ravindra Kumar Portfolio</title>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

	<link href="https://fonts.googleapis.com/css?family=Poppins:100,200,300,400,500,600,700,800,900" rel="stylesheet">

	<link rel="stylesheet" href="css/open-iconic-bootstrap.min.css">
	<link rel="stylesheet" href="css/animate.css">

	<link rel="stylesheet" href="css/owl.carousel.min.css">
	<link rel="stylesheet" href="css/owl.theme.default.min.css">
	<link rel="stylesheet" href="css/magnific-popup.css">

	<link rel="stylesheet" href="css/aos.css">

	<link rel="stylesheet" href="css/ionicons.min.css">

	<link rel="stylesheet" href="css/flaticon.css">
	<link rel="stylesheet" href="css/icomoon.css">
	<link rel="stylesheet" href="css/style.css">



	<style>
		/*======================================
//--//-->   ABOUT
======================================*/

		.about-mf .box-shadow-full {
			padding-top: 4rem;
			padding-bottom: 4rem;
		}

		.about-mf .about-img {
			margin-bottom: 2rem;
		}

		.about-mf .about-img img {
			margin-left: 10px;
		}


		.skill-mf .progress {
			/* background-color: #cde1f8; */
			margin: .5rem 0 1.2rem 0;
			border-radius: 0;
			height: .7rem;
		}

		.skill-mf .progress .progress-bar {
			height: .7rem;
			background-color: #ffbd39;
		}


		/* Animation styles */
		#typing-animation {
			position: relative;
			font-size: 30px;
			font-weight: bold;
			color: rgb(255, 255, 255);
			overflow: hidden;
			white-space: nowrap;
			animation: typing 3s steps(20, end) infinite;
		}

		#typing-animation:before {
			content: "";
			/* position: absolute; */
			top: 0;
			left: 0;
			width: 0;
			height: 100%;
			background-color: #ccc;
			animation: typing-cursor 0.5s ease-in-out infinite;
		}

		@keyframes typing {
			from {
				width: 0;
			}

			to {
				width: 100%;
			}
		}

		@keyframes typing-cursor {
			from {
				width: 5px;
			}

			to {
				width: 0;
			}
		}


		/* project image zoom effect */

		.zoom-effect {
			overflow: hidden;
			transition: transform 0.3s ease-out;
		}

		.zoom-effect:hover {
			transform: scale(1.1);
		}
	</style>


</head>

<body data-spy="scroll" data-target=".site-navbar-target" data-offset="300">


	<nav class="navbar navbar-expand-lg navbar-dark ftco_navbar ftco-navbar-light site-navbar-target" id="ftco-navbar">
		<div class="container">
			<a class="navbar-brand" href="index.html">Ravindra Kumar</a>
			<button class="navbar-toggler js-fh5co-nav-toggle fh5co-nav-toggle" type="button" data-toggle="collapse"
				data-target="#ftco-nav" aria-controls="ftco-nav" aria-expanded="false" aria-label="Toggle navigation">
				<span class="oi oi-menu"></span> Menu
			</button>

			<div class="collapse navbar-collapse" id="ftco-nav">
				<ul class="navbar-nav nav ml-auto">
					<li class="nav-item"><a href="#home-section" class="nav-link"><span>Home</span></a></li>
					<li class="nav-item"><a href="#about-section" class="nav-link"><span>About</span></a></li>
					<li class="nav-item"><a href="#resume-section" class="nav-link"><span>Resume</span></a></li>
					<li class="nav-item"><a href="#project-section" class="nav-link"><span>Projects</span></a></li>
					<li class="nav-item"><a href="#contact-section" class="nav-link"><span>Contact</span></a></li>
				</ul>
			</div>
		</div>
	</nav>
	<section id="home-section" class="hero">
		<div class="home-slider  owl-carousel">
			<div class="slider-item ">
				<div class="overlay"></div>
				<div class="container">
					<div class="row d-md-flex no-gutters slider-text align-items-end justify-content-end"
						data-scrollax-parent="true">
						<div class="one-third js-fullheight order-md-last img"
							style="background-image:url(images/RaviG.png);">
							<div class="overlay"></div>
						</div>
						<div class="one-forth d-flex  align-items-center ftco-animate"
							data-scrollax=" properties: { translateY: '70%' }">
							<div class="text">
								<span class="subheading">Hello!</span>
								<h1 class="mb-4 mt-3">I'm <span>Ravindra Kumar</span></h1>

								<!-- Element to contain animated typing -->
								<span id="typing-animation"></span>

								<script>

									// Initialize the typing animation
									const typingAnimationElement = document.getElementById('typing-animation');

									// Create an array of typing text
									const typingTexts = [
										'Front-End Developer ',
										'Web Designer  ',
										'Graphic Designer   ',
									];

									// Create a function to display the typing animation for a given text
									function playTypingAnimation(text) {
										// Loop through each character and add it to the element
										for (let i = 0; i < text.length; i++) {
											setTimeout(() => {
												typingAnimationElement.textContent += text[i];
											}, i * 200); // Increase the delay to slow down the typing animation
										}

										// Once the animation is complete, reset the text and start over
										setTimeout(() => {
											typingAnimationElement.textContent = '';
											playTypingAnimation(typingTexts[(typingTexts.indexOf(text) + 1) % typingTexts.length]);
										}, text.length * 200);
									}

									// Start the typing animation loop
									playTypingAnimation(typingTexts[0]);

								</script>

								<br>
								<br>
								<h2>A Fresher Student</h2>
								<!-- <h2 class="d-flex" style="margin-bottom: 0">With over 5 years of experience</h2> -->
								<!-- <br> -->
								<p><a href="https://www.youtube.com/@Knowledgecrossing"
										class="btn btn-primary py-3 px-4">YouTube</a>
									<a href="https://github.com/ravindrachy"
										class="btn btn-white btn-outline-white py-3 px-4">My works</a>
								</p>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>



	<section class="ftco-about img ftco-section ftco-no-pb" id="about-section">
		<div class="container">
			<div class="row">
				<div class="row d-flex align-items-stretch">
					<!-- <div class="row d-flex"> -->
					<div class="col-md-6 col-lg-5 d-flex">
						<div class="img-about img d-flex align-items-stretch">
							<div class="overlay">
								<div class="row">
									<div class="col-sm-6 col-md-5">
										<div class="about-img">
											<img src="images/about-me.jpg" class="img-fluid rounded b-shadow-a" alt="">
										</div>
									</div>
									<!-- Details next to profile image -->
									<div class="col-sm-6 col-md-7">
										<div class="about-info">
											<p><span class="title-s">Name: </span> <span>Ravindra Kumar</span></p>
											<p><span class="title-s">Job Role: </span> <span>Front-End Developer</span>
											</p>
											<p><span class="title-s">Experience: </span> <span>Fresher</span></p>
											<p><span class="title-s">Address: </span> <span>New Delhi, India</span></p>
										</div>
									</div>
								</div>

								<div class="skill-mf">
									<p class="title-s">Skills</p>
									<span>HTML5</span> <span class="pull-right">90%</span>
									<div class="progress">
										<div class="progress-bar" role="progressbar" style="width: 95%;"
											aria-valuenow="95" aria-valuemin="0" aria-valuemax="100"></div>
									</div>

									<span>CSS3</span> <span class="pull-right">85%</span>
									<div class="progress">
										<div class="progress-bar" role="progressbar" style="width: 85%"
											aria-valuenow="85" aria-valuemin="0" aria-valuemax="100"></div>
									</div>

									<span>JAVASCRIPT</span> <span class="pull-right">80%</span>
									<div class="progress">
										<div class="progress-bar" role="progressbar" style="width: 90%"
											aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
									</div>

									<span>BOOTSTRAP</span> <span class="pull-right">80%</span>
									<div class="progress">
										<div class="progress-bar" role="progressbar" style="width: 85%"
											aria-valuenow="85" aria-valuemin="0" aria-valuemax="100"></div>
									</div>

									<span>ADOBE PHOTOSHOP</span> <span class="pull-right">85%</span>
									<div class="progress">
										<div class="progress-bar" role="progressbar" style="width: 80%"
											aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
									</div>
								</div>
							</div>
						</div>
					</div>

					<div class="col-md-6 col-lg-7 pl-lg-5 pb-5">
						<div class="row justify-content-start pb-3">
							<div class="col-md-12 heading-section ftco-animate">

								<h1 class="big">About</h1>
								<h2 class="mb-4">About Me</h2>

								<p>I am Highly motivated and eager fresher with a strong educational background in the
									field of Front-End Development & Web Designing, accompanied by a bachelor's degree
									in Computer Science.
									Proficient in Front-End Development, Web Designing, Graphic Designing, and a passion
									for entering the IT industry.possess excellent communication skills, a keen
									attention to detail, and a willingness to learn and grow in a fast-paced
									environment.seeking a challenging role where I can utilise my skills and knowledge
									to contribute to the success of a dynamic organization.</p>
								<ul class="about-info mt-4 px-md-0 px-2">
									<li class="d-flex"><span>Profile:</span> <span>Front-End Development &amp; Web
											Designing</span>
									</li>
									<li class="d-flex"><span>Domain:</span> <span>Retail, Ecommerce, BFSI &amp; Digital
											Marketing</span></li>
									<li class="d-flex"><span>Education:</span> <span>Bachelor of Arts(Computer +
											English)</span></li>
									<li class="d-flex"><span>Language:</span> <span>English, Hindi</span></li>
									<li class="d-flex"><span>BI Tools:</span> <span>Microsoft Power BI, Looker &amp;
											Tableau</span></li>
									<li class="d-flex"><span>Other Skills:</span> <span>MS Word, Excel,Adobe Photoshop,
											Coreldraw, Adobe illustrator, Adobe Indesign, Git,
											Wordpress &amp; SEO</span></li>
									<li class="d-flex"><span>Interest:</span> <span>Traveling, Travel Photography,
											Teaching</span></li>

								</ul>
							</div>
						</div>


						<div class="counter-wrap ftco-animate d-flex mt-md-3">
							<div class="text">
								<p class="mb-4">
									<span class="number" data-number="2">0</span> <span>+</span>
									<span>&nbsp; Projects completed</span>
								</p>
								<p><a href="https://www.linkedin.com/in/ravindra-kumar-54050822b/"
										class="btn btn-primary py-3 px-3">LinkedIn</a></p>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>

			<br>
			<br>

			<div class="row">
				<h1 class="big-4">Education</h1>
				<div class="underline"></div>
			</div>
			<br>

			<div class="row">
				<div class="col-md-6">
					<div class="resume-wrap ftco-animate">
						<span class="date">2021-2024</span>
						<h2>Bachelor of Computer Science</h2>
						<span class="position"> University Of Delhi</span>
						<p class="mt-4">Grade: First class distinction.</p>
					</div>
				</div>


				<div class="row justify-content-center mt-5">
					<div class="col-md-6 text-center ftco-animate">
						<p><a href="D:\Download\Portfolio-Website-Template-main\Portfolio-Website-Template-main\images\Resume Ravindra kumar.pdf"
								class="btn btn-primary py-4 px-5">Download CV</a></p>
					</div>
				</div>
			</div>
	</section>



	<section class="ftco-section" id="project-section">
		<div class="container">
			<div class="row justify-content-center mb-5 pb-5">
				<div class="col-md-7 heading-section text-center ftco-animate">
					<h1 class="big big-2">Projects</h1>
					<h2 class="mb-4">Projects</h2>
					<p>Below are the sample amazon projects.</p>
				</div>
			</div>
			<div class="row d-flex">
				<div class="col-md-4 d-flex ftco-animate">
					<div class="blog-entry justify-content-end">
						<a href="#" class="block-20 zoom-effect" style="background-image: url('images/proj_1.png');">
						</a>
						<div class="text mt-3 float-right d-block">

							<h3 class="heading"><a href="#">
									amazon online shopping website using HTML, CSS, JAVASCRIPT</a></h3>
							<p>The Amazon project aims to revolutionize the way people shop with its vast online
								marketplace, fast delivery options, and convenient shopping experience. It has
								transformed the way people buy and sell goods, making it one of the most successful
								e-commerce platforms in the world. With its constant innovation and customer-centric
								approach, Amazon continues to dominate the online retail space and set new standards for
								the industry.</p>
						</div>
					</div>
				</div>
				<div class="col-md-4 d-flex ftco-animate">
					<div class="blog-entry justify-content-end">
						<a href="#"
							class="block-20 zoom-effect" style="background-image: url('images/proj_2.png');">
						</a>
						<div class="text mt-3 float-right d-block">

							<h3 class="heading"><a
									href="#">
									 Piza website using HTML, CSS, JAVASCRIPT</a></h3>
							<p>The pizza project aims to explore different pizza recipes, flavors, and toppings.
								It will involve experimenting with various dough recipes, sauce combinations, and cooking techniques.
								Ultimately, the goal is to create the perfect pizza that satisfies all taste buds..</p>
						</div>
					</div>
				</div>
	</section>



	<section class="ftco-section contact-section ftco-no-pb" id="contact-section">
		<div class="container">
			<div class="row justify-content-center mb-5 pb-3">
				<div class="col-md-7 heading-section text-center ftco-animate">
					<h1 class="big big-2">Contact</h1>
					<h2 class="mb-4">Contact Me</h2>
					<p>Below are the details to reach out to me!</p>
				</div>
			</div>

			<div class="row d-flex contact-info mb-5">
				<div class="col-md-6 col-lg-3 d-flex ftco-animate">
					<div class="align-self-stretch box p-4 text-center">
						<div class="icon d-flex align-items-center justify-content-center">
							<span class="icon-map-signs"></span>
						</div>
						<h3 class="mb-4">Address</h3>
						<p>New Delhi, India</p>
					</div>
				</div>
				<div class="col-md-6 col-lg-3 d-flex ftco-animate">
					<div class="align-self-stretch box p-4 text-center">
						<div class="icon d-flex align-items-center justify-content-center">
							<span class="icon-phone2"></span>
						</div>
						<h3 class="mb-4">Contact Number</h3>
						<p><a href="6203887247">6203887247</a></p>
					</div>
				</div>
				<div class="col-md-6 col-lg-3 d-flex ftco-animate">
					<div class="align-self-stretch box p-4 text-center">
						<div class="icon d-flex align-items-center justify-content-center">
							<span class="icon-paper-plane"></span>
						</div>
						<h3 class="mb-4">Email Address</h3>
						<p><a href="mailto:info@yoursite.com">919ravindrakumar@gmail.com</a></p>
					</div>
				</div>
				<div class="col-md-6 col-lg-3 d-flex ftco-animate">
					<div class="align-self-stretch box p-4 text-center">
						<div class="icon d-flex align-items-center justify-content-center">
							<span class="icon-globe"></span>
						</div>
						<h3 class="mb-4">Download Resume</h3>
						<p><a href="#">resumelink</a></p>
					</div>
				</div>

				<div class="container">
					<br>
					<br>
					<div class="row justify-content-center">
						<div class="col-md-7 ftco-animate text-center">
							<h2>Have a<span> Question? </span> <a href="" class="btn btn-primary py-3 px-5">Click
									Here</a> </h2>
						</div>
					</div>
					<br>
					<ul class="ftco-footer-social list-unstyled d-flex justify-content-center align-items-center mb-0">
						<li class="ftco-animate normal-txt">Find me on </li>
						<li class="ftco-animate"><a href="https://www.youtube.com/@Knowledgecrossing"><span
									class="icon-youtube"></span></a></li>
						<li class="ftco-animate"><a href="https://www.linkedin.com/in/ravindra-kumar-54050822b"><span
									class="icon-linkedin"></span></a></li>
						<li class="ftco-animate"><a href="https://twitter.com/Ravindra62033"><span
									class="icon-twitter"></span></a></li>
						<li class="ftco-animate"><a href="https://www.facebook.com/profile.php?id=100030472993196"><span
									class="icon-facebook"></span></a></li>
						<li class="ftco-animate"><a href="https://www.instagram.com/ravi_chaudhary_32/"><span
									class="icon-instagram"></span></a></li>
					</ul>
					<br>
				</div>
			</div>
	</section>




	<footer class="ftco-footer ftco-section">
		<div class="container">
			<div class="row">
				<div class="col-md-12 text-center">

					<p><!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
						Copyright &copy;
						<script>document.write(new Date().getFullYear());</script> All rights reserved | This template
						is made with <i class="icon-heart color-danger" aria-hidden="true"></i> by <a
							href="https://colorlib.com" target="_blank">Colorlib</a>
						<!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
					</p>
				</div>
			</div>
		</div>
	</footer>


	<!-- loader -->
	<div id="ftco-loader" class="show fullscreen"><svg class="circular" width="48px" height="48px">
			<circle class="path-bg" cx="24" cy="24" r="22" fill="none" stroke-width="4" stroke="#eeeeee" />
			<circle class="path" cx="24" cy="24" r="22" fill="none" stroke-width="4" stroke-miterlimit="10"
				stroke="#F96D00" />
		</svg></div>


	<script src="js/jquery.min.js"></script>
	<script src="js/jquery-migrate-3.0.1.min.js"></script>
	<script src="js/popper.min.js"></script>
	<script src="js/bootstrap.min.js"></script>
	<script src="js/jquery.easing.1.3.js"></script>
	<script src="js/jquery.waypoints.min.js"></script>
	<script src="js/jquery.stellar.min.js"></script>
	<script src="js/owl.carousel.min.js"></script>
	<script src="js/jquery.magnific-popup.min.js"></script>
	<script src="js/aos.js"></script>
	<script src="js/jquery.animateNumber.min.js"></script>
	<script src="js/scrollax.min.js"></script>

	<script src="js/main.js"></script>

</body>

</html>
