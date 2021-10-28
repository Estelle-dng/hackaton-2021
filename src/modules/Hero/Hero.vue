<template>
  <section class="main">
  <Wrapper>
      <section class="card-lg__container">
        <p class="card__text-sm">Mosae - Votre guide culturel Bordelais</p>
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
        <section class="card-sm" style="background-image:url('https://images.unsplash.com/photo-1584962356612-f7092400e895?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=600&q=60')">
          <p class="card__text-sm">Tanifa - Spain</p>
          <h1 class="card__text-lg">Los Lances Beach</h1>
        </section>
        <!--- END: CARD --->

        <!--- START: CARD --->
        <section class="card-sm" style="background-image: url('https://images.unsplash.com/photo-1489823480956-0204142cfebd?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=600&q=60'); background-position: center right;">
          <p class="card__text-sm">Japan Alps</p>
          <h1 class="card__text-lg">Nagano Prefecture</h1>
        </section>
        <!--- END: CARD --->

        <!--- START: CARD --->
        <section class="card-sm" style="background-image: url('https://images.unsplash.com/photo-1527549993586-dff825b37782?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=600&q=60')">
          <p class="card__text-sm">Sierra Nevada - USA</p>
          <h1 class="card__text-lg">Yosemite National  </h1>
        </section>
        <!--- END: CARD --->

        <!--- START: CARD --->
        <section class="card-sm" style="background-image: url('https://images.unsplash.com/photo-1537431701805-c1bb45cd2f92?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=600&q=60')">
          <p class="card__text-sm">Cappadocia - Turkey</p>
          <h1 class="card__text-lg">Goreme &nbsp; Valley</h1>
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
  border: 1px solid rgba(255,255,255,0.5);
  border-radius: 24px;
  font-size: 14px;
  text-align: center;
  text-decoration: none;
  text-transform: uppercase;
  width: 100px;
  margin: 8px 0 0;
  opacity: 0.5;
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
  font-size: 22px;
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
    font-size: 40px;
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
    opacity: 0.5;
  }
  .card__text-sm {
    font-size: 15px;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .card__text-sm::before {
    width: 24px;
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
  box-shadow: inset 0 0 100vw 100vw rgba(0, 0, 0, 0.3),
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
// .main::-webkit-scrollbar {
//   display: none;
// }

// .main {
//   -ms-overflow-style: none;
// }
</style>
