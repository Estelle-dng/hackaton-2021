<template>
  <div class="step-container">
    <div class="number-container">
      <p class="pre-number">.0</p>
      <p class="number">{{ number }}</p>
    </div>
    <div class="text-infos">
      <h3 class="title">{{ title }}</h3>
      <p class="text">{{ text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Steps",

  props: {
    text: { type: String, required: true },
    title: { type: String, required: true },
    number: { type: String, required: true },
  },
};
</script>

<style lang="scss" scoped>
.step-container {
  display: flex;
  width: 100%;
  .number-container {
    font-family: $ff-lust;
    display: flex;
    color: $dark-gray;
    margin-right: 18px;
    .pre-number {
      line-height: unset;
      font-size: 50px;
      font-family: $ff-lust;
      margin-top: 12px;
    }
    .number {
      line-height: unset;
      font-family: $ff-lust;
      font-size: 77px;
    }
  }
  .text-infos {
    text-align: left;
    padding-right: 16px;
    margin-bottom: 58px;
    .title {
      font-weight: 600;
      color: $dark-gray;
      margin-bottom: 16px;
    }
    .text {
      font-weight: 300;
      font-size: 16px;
    }
  }
}
@media screen and (max-width: 768px) {
  .step-container {
    display: block;
    .number-container {
      margin-bottom: 17px;
      justify-content: center;
    }
    .text-infos {
      text-align: center;
      padding-right: 0;
      .title {
        font-size: 22px;
        line-height: 25px;
        margin-bottom: 12px;
      }
      .text {
        margin-bottom: 36px;
        line-height: 18px;
      }
    }
  }
}
</style>
