<template>
  <section class="main">
  <Wrapper>
      <section class="card-lg__container">
        <p class="card__text-sm">Mosaë - Votre guide culturel Bordelais</p>
        <h1 class="card__text-lg">Découvrir l'art de la ville</h1>
        <p class="card__text-md">Trouvez les évènements culturels près de chez vous.</p>
        <div class="d-flex">
          <a href="#" class="card__btn">IOS</a>
          <a href="#" class="card__btn">Android</a>
          <a href="#" class="card__btn">Desktop</a>
        </div>
      </section>

      <section class="card-sm__container">
        <!--- START: CARD --->
        <section class="card-sm" style="background-image:url('/img/accueil.png')">
          <p class="card__text-sm">Une selection</p>
          <h6 class="card__text-lg">Personnalisée d'oeuvres originales chaque semaine</h6>
        </section>
        <!--- END: CARD --->

        <!--- START: CARD --->
        <section class="card-sm" style="background-image:url('/img/profil.png')">
          <p class="card__text-sm">Un profil</p>
          <h6 class="card__text-lg">Avec votre planning d'évènements</h6>
        </section>
        <!--- END: CARD --->

        <!--- START: CARD --->
        <section class="card-sm" style="background-image:url('/img/evenement.png')">
          <p class="card__text-sm">Des évènements</p>
          <h6 class="card__text-lg">Détaillés et exclusifs</h6>
        </section>
        <!--- END: CARD --->

        <!--- START: CARD --->
        <section class="card-sm" style="background-image:url('/img/calendrier.png')">
          <p class="card__text-sm">Un calendrier</p>
          <h6 class="card__text-lg">Détaillé des évènements dans votre ville</h6>
        </section>
        <!--- END: CARD --->
      </section>
  </Wrapper>
  </section>
</template>

<script>
import Wrapper from '@/components/Wrapper';
export default {
  name: "Navbar",
  components:{
    Wrapper
  }
};
</script>

<style lang="scss" scoped>
#main-wrapper{
  display: flex;
  height: calc(100vh - 100px);
}
/*CARD*/
.card__btn {
  color: #fff;
  border: 1px solid rgba(255,255,255,0.8);
  border-radius: 24px;
  font-size: 14px;
  text-align: center;
  text-decoration: none;
  text-transform: uppercase;
  width: 100px;
  margin: 8px 0 0;
  opacity: 0.8;
  padding: 8px;
  margin-right: 15px;
  &:hover {
    transform: scale(0.95);
    transition: 0.6s ease;
  }
}
.card__text-sm {
  color: #fff;
  font-size: 18px;
  margin: 0;
  padding: 16px 0 8px;
  position: relative;
  overflow: hidden;
  text-overflow: ellipsis;
}
.card__text-sm::before {
  content: "";
  background: #fff;
  height: 1px;
  width: 16px;
  position: absolute;
  top: 0;
}
.card__text-lg {
  color: #fff;
  font-size: 15px;
  font-weight: 300;
  text-transform: uppercase;
  line-height: 1.2;
  width: 100%;
  margin: 0;
  overflow: hidden;
  text-overflow: ellipsis;
}
/*...large...*/
.card-lg__container {
  padding: 0 16px 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  overflow-x: scroll;

  .card__text-lg {
    font-size: 20px;
    font-weight: 400;
    letter-spacing: 1.4px;
    overflow: hidden;
    text-overflow: ellipsis;
  } 
  .card__text-md {
    color: #fff;
    font-size: 15px;
    font-weight: 100;
    line-height: 1.5;
    padding: 0 32px 0 0;
    opacity: 0.8;
  }
  .card__text-sm {
    font-size: 15px;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .card__text-sm::before {
    width: 15px;
    height: 2px;
  }
}
/*...small...*/
.card-sm__container {
  height: 300px;
  margin: 0 -125px 0 0;
  display: flex;
  align-self: center;
  overflow-x: scroll;
}
.card-sm {
  background: #ccc;
  background-size: cover; 
  background-position: center center;
  box-shadow: inset 0 0 100vw 100vw rgba(0, 0, 0, 0.5),
    0 16px 8px -8px rgba(0,0,0,0.4);
  border-radius: 8px;
  width: 150px;
  height: calc(100% - 64px); 
  margin: 0 8px;
  padding: 24px 16px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  cursor: pointer;
  transition: 0.3s ease;
  
  &:hover {
    margin: -8px 8px 0;
  }
  
  .card__text-sm { 
    opacity: 0.8;
  }
  
}


/*HIDE DEFAULT SCROLL BAR*/
.card-sm__container::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for Chrome, Safari and Opera */
.card-sm__container::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for IE, Edge and Firefox */
.card-sm__container {
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}

.card-sm__container {
  -ms-overflow-style: none;
}
</style>
