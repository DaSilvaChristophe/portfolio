<template>
  <section id="presentation" class="container-fluid transition_page">
    <div class="mx-auto ligne mb-5"></div>
    <div class="d-flex ">
        <div class="col-4 bg-light d-flex justify-content-center align-items-center h-75">
            <img  class="rounded" src="../assets/christophe_da_silva.jpg" alt="developpeur web freelance">
        </div>
        <article class="col-8 text bg-white">
          <h2 class="h1 pt-4 pb-3 mx-auto">Qui suis-je ?</h2>
          <p class="pt-2 mx-auto">
            Tout d'abord bonjour à tous et bienvenue à vous, je me présente je m’appelle Christophe (vous pouvez m'appeler Cris 😉) développeur Full Stack passionné par le développement web.
            <br><br>
            Je mets mes compétences et mon savoir-faire au service d’entreprises, entrepreneurs et/ou particuliers qui souhaite créer leur site, développer de nouveaux concepts ou simplement intégrer de nouvelles fonctionnalités sur site existant, que ce soit pour le développement de business où à titre personnel.
            <br><br>
            Vous trouverez mes services proposés  et mes compétences techniques juste en dessous ⬇️ N'hésitez donc pas à me contacter pour vos besoins.
            <br><br>
            Merci d'avoir pris le temps de lire ces quelques lignes et au plaisir d'échanger avec vous 🙂.
          </p>
        </article>
    </div>
  </section>
</template>

<script>

export default {
  name: 'Presentation',
  }
  
</script>
  
<style scoped>

  .ligne {
    width: 100%;
    margin-right: 5%;
    height: 1px;
    background-color: #999999;
    opacity: 1;
  }

  img
  {
    object-fit: cover;
    height: 450px;
  }
  
  .text h2
  {
    font-family:  Helvetica, Arial, sans-serif;
    width: 70%;
    font-size: 1.8em;
    font-weight: 500;
    color: rgb(25, 29, 25);
    text-align: center;
  }
  .text p
  {
    width: 100%;
    font-size: 1.1em;
    color: rgb(25, 29, 25);
    font-weight: 400;
    max-width: 800px;
  }
  
  /* Animation transition page */
  
  .transition_page {
    animation: opacity 3s linear forwards;
  }
  
  @keyframes opacity {
  0% {
      opacity: 0;
    }
    50% {
      opacity: 0.7;
    }
    100% {
      opacity: 1;
    }
  }
  
</style>