<template>
  <div id="partners" class="partners d-flex">
<Wrapper>
      <div class="w50">
        <img src="../../../public/img/feature-desktop.png" alt="">
      </div>
      <div class="w50">
        <h3>DEVENIR PARTENAIRES</h3>
        <h4>Faites découvrir vos évènements facilement.</h4>
        <p>Vous représentez une ville, une organisation et vous souhaitez utiliser Mosae pour promouvoir votre art ? Faites une demande de partenariat via le formulaire ci-dessous et nous vous recontacterons très rapidement.</p>
        <Button
              :isRouter="false"
              text="Proposez vos évènements"
              ariaLabel="partner"
              link="#contact"
              className="nav-button"
              classA="nav-a"
              />
      </div>
  </Wrapper>
    </div>
</template>

<script>
import Button from '@/components/Button';
import Wrapper from '@/components/Wrapper';
export default {
  name: "Partners",
  components:{Button, Wrapper}
};
</script>

<style lang="scss" scoped>
.partners{
  background-color: $dark-gray;
  background-image: url("../../../public/img/hero.jpg");
  box-shadow: inset 0 0 100vw 100vw rgb(0 0 0 / 75%), 0 16px 8px -8px rgb(0 0 0 / 40%);
  #main-wrapper{
    color: $ice;
    padding-top:100px;
    padding-bottom: 80px;
    display: flex;
  .w50:first-child{padding-right: 15px;}
  .w50:last-child{
    padding-left: 15px;
    margin-top: 55px;
    }
  h3{margin-bottom: 15px;}
  h4, p{
    margin-bottom: 50px;
    opacity: 0.8;
  }
  img{
    height: 100%;
    width: 100%;
    object-fit: contain;
    object-position: center;
  }
  }
}
</style>
