<template>
  <div class="newsletter">
    <Wrapper>
          <h5>Abonnez vous à notre newletter</h5>
          <h6>Pour rester au courant des nouveautés</h6>
          <form action="">
            <input type="text" placeholder="Votre Mail">
            <input type="text" placeholder="Votre Nom">
            <Button
                :isRouter="false"
                text="S'abonner"
                ariaLabel="partner"
                link="#partner"
                className="button-secondary"
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
.newsletter{
  color: $ice;
  text-align: center;
  background: url(../../../public/img/newsletter-bg.jpg) top center no-repeat;
  background-size: cover;
  padding:100px 0;
  width: 100vw;
  height: 300px;
  h5,h6{margin-bottom: 15px;}
  form{ 
    justify-content: center;
    margin: 0 auto;
    display: flex;
    input{
      background: rgba(255,255,255,0.8);
      border-radius: 5px;
      padding: 12px 16px;
      font-size: 12px;
      text-transform: uppercase;
      border: 0;
      color: #707070;
      width: 160px;
      margin-right: 8px;
    }
  }
}
</style>
