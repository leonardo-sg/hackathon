<template>
  <div class="home">
    <div class="client__card">
      <CardClient />
    </div>
    <br />
    <div class="benefits__card">
      <span>Beneficios deste nível</span>
      <img :src="icon" alt="" />
    </div>
    <div class="new__delivery">
      <NewDelivery />
      <NewDeliveryTwo />
      <br />
      <span class="see__more">Ver mais entregas programadas</span>.
      <br />
      <br />
      <span class="points__earn">Ganhe mais pontos</span>
      <br />
      <div class="home__carroussel">
        <a-carousel :after-change="onChange" dots="false">
          <HelthPoints />
          <DogHeroPoints />
          <VaccinePoints />
        </a-carousel>
      </div>
      <br />
    </div>
  </div>
</template>

<script>
import CardClient from "../components/client/cardClient.vue";
import NewDelivery from "../components/client/newDelivery.vue";
import NewDeliveryTwo from "../components/client/newDeliveryTwo.vue";
import HelthPoints from "../components/cardPoints/helthPoints.vue";
import DogHeroPoints from "../components/cardPoints/dogHeroPoints.vue";
import VaccinePoints from "../components/cardPoints/vaccinePoints.vue";
import Group from "../assets/icons/GroupVantage.svg";

export default {
  name: "Home",
  components: {
    CardClient,
    NewDelivery,
    NewDeliveryTwo,
    HelthPoints,
    DogHeroPoints,
    VaccinePoints,
  },
  data() {
    return {
      icon: Group,
    };
  },
};
</script>

<style scoped>
@media (max-width: 600px) {
  .home {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #e5e5e5;
  }
  .client__card {
    display: flex;
    justify-content: center;
    margin-top: 1rem;
  }
  .benefits__card {
    width: 90%;
    display: flex;
    justify-content: center;
    align-items: center;
    font-style: normal;
    font-weight: 600;
    font-size: 20px;
    line-height: 27px;
    display: flex;
    flex-direction: column;

    color: #000000;
  }
  .new__delivery {
    width: 100%;
    background-color: #ffffff;
  }
  .see__more {
    font-style: normal;
    font-weight: 600;
    font-size: 14px;
    line-height: 19px;
    text-align: center;
    color: #582d89;
  }
  .points__earn {
    padding: 0 0 0 1rem;
    display: flex;
    font-style: normal;
    font-weight: 600;
    font-size: 20px;
    line-height: 27px;
    color: #000000;
  }

  .ant-carousel >>> .slick-slide {
    overflow: hidden;
  }
  .slick-dots slick-dots-bottom {
    display: none !important;
  }

  .home__carroussel {
    margin: 0.5rem;
  }
}
</style>
