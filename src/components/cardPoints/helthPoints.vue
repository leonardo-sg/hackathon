<template>
  <div class="card__shape">
    <div class="card__image">
      <img class="image" :src="iconDog" alt="" />
    </div>
    <div class="content__card">
      <span class="card__title">O melhor plano de saúde</span>
      <span class="card__subtitle">
        Contrate um plano de saúde da PortoPet e garanta o bem estar do seu pet
        para todas aventuras.
      </span>
    </div>
    <div>
      <a-button class="btn__plan" type="primary">
        Contratar plano de saúde
      </a-button>
    </div>
  </div>
</template>

<script>
import Dog from "@/assets/icons/DogHelth.svg";
export default {
  name: "helthPet",
  data() {
    return {
      iconDog: Dog,
    };
  },
};
</script>

<style scoped>
.card__shape {
  border: solid 1px rgba(221, 221, 221, 1);
  border-radius: 10px;
  display: flex;
  flex-direction: column;
}

.card__title {
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 25px;
  color: #000000;
  display: flex;
}

.card__subtitle {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 19px;
  color: #000000;
  display: flex;
  text-align: initial;
}

.card__image {
  width: 100%;
}

.content__card {
  margin: 1rem;
}

.btn__plan {
  width: 95%;
  height: 40px;
  background: #582d89;
  margin: 0.5rem;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 19px;
  text-align: center;

  color: #ffffff;
}

.image {
  width: 100%;
}
</style>
