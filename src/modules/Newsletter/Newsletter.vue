<template>
  <div id="contact" class="contact">
    <Wrapper>
      <form action="">
          <h5>Devenez partenaire</h5>
          <p>Vous voulez devenir partenaire régulier ou nous faire découvrir un évènement ponctuel ? <br> N'hésitez pas à nous contacter en nous décrivant votre organisation et votre démarche, nous vous recontacterons pour en discuter !</p>
          
            <div class="d-flex">
              <input type="text" placeholder="Votre Mail">
              <input type="text" placeholder="Votre Nom">
            </div>
            <div class="d-flex">
              <input type="text" placeholder="Votre Organisation">
              <input type="text" placeholder="Votre Type de projet">
            </div>
            <textarea id="story" placeholder="">
              Renseignez une courte description de votre projet
            </textarea>
            <div>
              <p class="phone">Si vous souhaitez être contacté par téléphone :</p>
              <input type="text" placeholder="Votre Téléphone">
            </div>
            <Button
                :isRouter="false"
                text="Envoyer"
                ariaLabel="partner"
                link="#partner"
                className="button"
                classA="nav-a"
                />
            </form>
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
.contact{
  color: $ice;
  text-align: center;
  background: url(../../../public/img/newsletter-bg.jpg) top center no-repeat;
  background-size: cover;
  padding:100px 0;
  width: 100vw;
  h5,h6,p{
    color:$dark-gray;
    margin-bottom: 30px;
    }
  .phone{
    margin-bottom: 0;
  }  
  .button{margin-top:15px;}
  form{ 
    justify-content: center;
    margin: 0 auto;
    background-color: rgba(255,255,255,0.5);
    border-radius: 5px;
    padding: 25px;
    input, textarea{
      background: rgba(255,255,255,0.8);
      border-radius: 5px;
      padding: 12px 16px;
      font-size: 12px;
      text-transform: uppercase;
      border: 0;
      color: #707070;
      width: 200px;
      margin-right: 8px;
      margin: 15px;
    }
  }
  textarea{
    width: 95% !important;
    height: 150px;
    margin-left: 0 !important;
    font-family: $ff-spartan;
  }
}
</style>
