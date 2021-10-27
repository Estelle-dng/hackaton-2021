<template>
  <Wrapper>
    <div class="hero-container">
      <div class="hero-img">
        <!-- <img src="@/assets/img/hero_landing.jpg" alt="" /> -->
      </div>
      <div class="text-bloc">
        <h1 class="title">title</h1>
        <p class="text">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Saepe vitae
          cupiditate officia temporibus itaque non dolore qui eum deleniti
          voluptatibus, nemo quod? Eligendi labore delectus amet, laboriosam
          perferendis ea laudantium.
        </p>
        <div class="button-group">
          <Button
            isRouter
            ariaLabel="je suis un cta"
            link="#"
            text="je suis un cta"
            class="cta-button button-primary"
          />
          <Button
            :isRouter="false"
            ariaLabel="je suis un cta secondaire"
            link="#"
            text="cta secondary"
            class="cta-button button-secondary"
          />
        </div>
      </div>
    </div>
  </Wrapper>
</template>

<script>
import Button from "@/components/Button";
import Wrapper from "@/components/Wrapper";

export default {
  name: "Navbar",
  components: { Button, Wrapper },
};
</script>

<style lang="scss" scoped>
.hero-container {
  height: calc(100vh - 206px);
  .text-bloc {
    position: relative;
    max-width: calc(50vw - 120px);
    .title {
      color: $dark-gray;
    }
    .text {
      padding-top: 16px;
      font-size: 20px;
      font-weight: 300;
      line-height: 33px;
    }
    .cta-button {
      margin-top: 32px;
      margin-right: 6px;
    }
    .button-primary{border: 1px solid $purple;}
  }
  .hero-img {
    width: 100%;
    height: 100vh;
    position: absolute;
    right: 0;
    top: 0;
    z-index: -1;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }
}
@media screen and (max-width: 768px) {
  .hero-container {
    padding: 0 14px 70px 14px;
    .text-bloc {
      max-width: 100%;
      padding-top: 200px;
      .title {
        font-size: 32px;
        line-height: 36px;
        font-weight: 800;
      }
      .text {
        font-size: 18px;
        line-height: 33px;
      }
      .button-group {
        text-align: center;
        .cta-button {
          width: 66%;
        }
      }
    }
    .hero-img {
      position: relative;
      height: 15vh;
      img {
        position: absolute;
        height: 600px;
        width: auto;
        right: -14px;
      }
    }
  }
}
</style>
