<template>
    <section id="services" class="container">
		<div class="mx-auto ligne my-5"></div>
		<h1 class="text-center w-100 mb-5">SERVICES</h1>
		<div class="d-flex">
			<article class="col-3">
				<figure class="image-block">
				<img src="../assets/accompagnement.png" alt="main tendu pour aider l'autre"/>
				<figcaption class="figcaption_one">
					<h2>
						Accompagnement
					</h2>
					<p>Accompagnement dans le processus de création de votre projet, faisabilité, développment, production, post-production.</p>
				</figcaption>
				</figure>
			</article>
			<article class="col-3">
				<figure class="image-block">
				<img src="../assets/projet_web.png" alt="ordinateur en arrière plan mobile premier plan"/>
				<figcaption class="figcaption_two">
					<h2>
						Projet Web
					</h2>
					<p>Création/maintenance de site vitrine professionnel, E-commerce, Applications, API, Blog...</p>
				</figcaption>
				</figure>
			</article>
			<article class="col-3">
			<figure class="image-block">
			<img src="../assets/developpement.png" alt="langage de programmation"/>
			<figcaption class="figcaption_three">
				<h2>
					Developpement
				</h2>
				<p>Développement Full Stack & Intégration en langages de programmation (Vanilla & frameworks) ou CMS, création/maintenance de base de données, création d'API, optimisation SEO, responsive...</p>
			</figcaption>
			</figure>
		</article>
		<article class="col-3">
			<figure class="image-block">
			<img src="../assets/website.png" alt="site web sur ordinateur"/>
			<figcaption class="figcaption_four">
				<h2>
					Production
				</h2>
				<p>Mise en ligne sur environnement de test, mise en production, maintenance website...</p>
			</figcaption>
			</figure>
		</article>
		</div>
    </section>
</template>
  
<script> 

  export default {
    name: 'Services',
  }
  
</script>
  
<style lang="scss" scoped>

.ligne {
  width: 100%;
  margin-right: 5%;
  height: 1px;
  background-color: #999999;
  opacity: 1;
}

$base-duration: 500ms;

// Colors
$color-1: #2c3e50;
$color-2: #1abc9c;
$color-3: #2ecc71;

// Breakpoints
$sm: new-breakpoint(min-width 320px);
$med: new-breakpoint(min-width 768px);
$lg: new-breakpoint(min-width 1024px);

*, *:before, *:after {
	box-sizing: border-box;
	outline: none;
}

html {
	font-family: 'Roboto', sans-serif;
	font-size: 16px;
	font-smooth: auto;
	font-weight: 300;
	line-height: 1.5;
	color: #444;
}

body {
	position: relative;
	display: flex;
	align-items: center;
	justify-content: center;
	width: 100%;
	height: 100vh;
	// background-color:darken($color-1, 4%);
}

h1 {
	font-family:  Helvetica, Arial, sans-serif;
}

article {
	padding-left: 5px;
	padding-right: 5px;
}

figure {
	position: relative;
	display: flex;
	align-items: center;
	justify-content: center;
	width: 100%;
	height: 467px;
	border-radius: 10px;
	box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
	transition: all 0.3s cubic-bezier(.25,.8,.25,1);
	overflow: hidden;
	&:hover {
		box-shadow: 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
		img {
			transform: scale(1.25);
		}
		figcaption {
			bottom: 0;
		}
	}
	img {
		height: 100%;
		object-fit: cover;
		transition: 0.25s;
	}
	.figcaption_one{
		position: absolute;
		bottom: -31%;
		left: 0;
	}
	.figcaption_two{
		position: absolute;
		bottom: -25.5%;
		left: 0;
	}
	.figcaption_three{
		position: absolute;
		bottom: -48%;
		left: 0;
	}
	.figcaption_four{
		position: absolute;
		bottom: -25.5%;
		left: 0;
	}
	figcaption {
		width: 100%;
		//height: 50%;
		margin: 0;
		padding: 30px;
		background-color: rgba(black,0.85);
		box-shadow: 0 0 20px rgba(black,0.4);
		color: white;
		line-height: 1;
		transition: 0.25s;
		h2 {
			font-family:  Helvetica, Arial, sans-serif;
			margin: 0 0 20px;
			padding: 0;
		}
		p {
			font-size: 15px;
			width: 95%;
			line-height: 1.75;
		}
		button {
			position: relative;
			display: flex;
			align-items: center;
			justify-content: center;
			margin: 10px 0 0;
			padding: 10px 30px;
			background-color: $color-2;
			border: none;
			border-radius: 5px;
			color: white;
			font-size: 14px;
		}
	}
}
 
</style>
  