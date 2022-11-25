<template>
    <section id="portfolio" class="container mb-5">
		<div class="mx-auto ligne my-5"></div>
		<h1 class="text-center w-100 mb-5">PORTFOLIO</h1>
		<div class="d-flex justify-content-center">
			<article class="col-6 mx-2 text-center bg-white rounded shadow">
                <h2 class="my-4 cil">ArtsCoeurInLoveAgency</h2>
                <a href="https://www.coeurinlove.com/" target="_blank">
				<figure class="image-block mx-auto">
				    <img src="../assets/coeurinlove.png" alt="main tendu pour aider l'autre"/>
                </figure>
                </a>
                <div class="size-paragraph">
                    <h3 class="border-bottom">Création/Maintenance CMS</h3>
                    <p class="pt-2">Accompagnement et réalisation du website de l'entreprise (CMS - Wix) pour une agence artistique basé sur Fontainebleau/Avon (77300). <br> Maintenance du site : amélioration/intègration sur le website a la demande client, SEO, gestion analytics et business (Google).. <br> Design réalisé en collaboration avec le client. <br><br> <strong>En collaboration depuis fév. 2020</strong></p>
                </div>
			</article>
			<article class="col-6 mx-2 text-center bg-white rounded shadow">
                <h2 class="my-4 bmw">BMW Contract</h2>
                <a href="https://www.test-restitution.fr" target="_blank">
				<figure class="image-block mx-auto">
				    <img src="../assets/bmw_project.png" alt="ordinateur en arrière plan mobile premier plan"/>
				</figure>
                </a>
                <div class="size-paragraph">
                    <h3 class="border-bottom">Intégration/Développement</h3>
                    <p class="pt-2">Réalisation/intégration sous maquette (Adobe XD) d'un website pour le groupe BMW via l'agence Duncan Paris. <br> Intégration HTML5/CSS3, Javascript Vanilla, Bootstrap V5, Amélioration du TDC, validé par le groupe BMW actuellement sur environnement de test.. <br><br> <strong>Validé par le groupe BMW <br>Actuellement sur environnement de test</strong></p>
                </div>
			</article>
		</div>
    </section>
</template>
  
<script> 

  export default {
    name: 'Portfolio',
  }
  
</script>
  
<style lang="scss" scoped>

@font-face {
  font-family: "BMWTypeNext Light";
  src: url("../assets/fonts/BMWTypeNext/TTF/BMWTypeNextTT-Light.ttf") format("ttf"),
    url("../assets/fonts/BMWTypeNext/EOT/BMWTypeNextTT-Light.eot") format("eot"),
    url("../assets/fonts/BMWTypeNext/WOFF/BMWTypeNextTT-Light.woff") format("woff"),
    url("../assets/fonts/BMWTypeNext/WOFF2/BMWTypeNext-Light.woff2") format("woff2");
}

@font-face {
  font-family: "BMWTypeNext Bold";
  src: url("../assets/fonts/BMWTypeNext/TTF/BMWTypeNextTT-Bold.ttf") format("ttf"),
    url("../assets/fonts/BMWTypeNext/EOT/BMWTypeNextTT-Bold.eot") format("eot"),
    url("../assets/fonts/BMWTypeNext/WOFF/BMWTypeNextTT-Bold.woff") format("woff"),
    url("../assets/fonts/BMWTypeNext/WOFF2/BMWTypeNext-Bold.woff2") format("woff2");
}

@font-face {
  font-family: "Vladimir";
  src: url("../assets/fonts/Vladimir/VladimirScript.ttf") format("ttf"),
    url("../assets/fonts/Vladimir/VladimirScript.eot") format("eot"),
    url("../assets/fonts/Vladimir/VladimirScript.woff") format("woff"),
    url("../assets/fonts/Vladimir/VladimirScript.woff2") format("woff2");
}

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
	height: 267px;
	border-radius: 10px;
	box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
	transition: all 0.3s cubic-bezier(.25,.8,.25,1);
	overflow: hidden;
	&:hover {
		box-shadow: 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
		img {
			transform: scale(1.03);
		}
	}
	img {
		height: 100%;
		object-fit: cover;
		transition: 0.25s;
	}
}

.image-block {
    width: 95%;
}

.cil {
    font-family: "Vladimir", Helvetica, Arial, sans-serif;
}

.bmw {
    font-family: "BMWTypeNext Bold", Helvetica, Arial, sans-serif;
}

h3 {
    font-family: Helvetica, Arial, sans-serif;
    padding-top: 7px;
    padding-bottom: 8px;
}

.size-paragraph {
    width: 90%;
    margin: auto;
    padding-bottom: 10px;
}

</style>
  