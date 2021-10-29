<template>
  <Wrapper>
    <div id="concept" class="steps-container">
      <h2 class="title">La culture à portée de clic</h2>
      <div class="steps">
        <Steps
          number="1"
          title="Des Weekly News"
          text="Découvrez chaque semaine une selection d'évènements et de lieux à visiter dan votre ville."
        />
        <Steps
          number="2"
          title="Un planning personnalisé"
          text="Sélectionnez les évènements qui vous intérèssent, nous vous créons un planning de vos futures visites."
        />
        <Steps
          number="3"
          title="À la découverte de l'inconnu"
          text="Profitez de la culture comme vous ne l'avez jamais connue, sous toutes ses formes et participez, vous aussi à l'agrandissement de notre planning !"
        />
      </div>
      <Button
        :isRouter="false"
        ariaLabel="Step"
        text="À propos"
        link="#about"
        class="button"
      />
    </div>
  </Wrapper>
</template>

<script>
import Button from "@/components/Button";
import Wrapper from "@/components/Wrapper";
import Steps from "@/modules/Steps";

export default {
  name: "StepsBloc",
  components: { Button, Steps, Wrapper },
};
</script>

<style lang="scss" scoped>
.steps-container {
  padding-top: 150px;
  padding-bottom: 150px;
  text-align: center;
  .title {
    padding-bottom: 71px;
    color: $purple;
    font-size: 32px;
  }
  .steps {
    display: flex;
  }
}
@media screen and (max-width: 768px) {
  .steps-container {
    padding: 0 14px 80px 14px;
    .title {
      font-size: 32px;
      line-height: 38px;
      padding-bottom: 44px;
    }
    .steps {
      display: block;
      margin-bottom: 36px;
    }
  }
}
</style>
