<template>
  <div class="content__delivery">
    <span class="section__title">
      Próximas entregas
    </span>
    <div class="card__delivery">
      <div>
        <span class="card__quantity">05</span>
        <span class="card__month">Set</span>
      </div>
      <div>
        <img class="card__icon" :src="iconTrue" />
        <img class="card__icon" :src="iconremedio" />
        <img :src="iconMaisDois" />
      </div>
      <div>
        <img :src="iconPontos" />
      </div>
    </div>
  </div>
</template>

<script>
import True from "@/assets/icons/true.svg";
import Remedio from "@/assets/icons/remedio.svg";
import Maisdois from "@/assets/icons/2icon.svg";
import Pontos from "@/assets/icons/pontos.svg";

export default {
  name: "newDelivery",
  data() {
    return {
      iconTrue: True,
      iconremedio: Remedio,
      iconMaisDois: Maisdois,
      iconPontos: Pontos,
    };
  },
};
</script>

<style scoped>
.section__title {
  padding: 0 0 0 1rem;
  display: flex;
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 27px;
  color: #000000;
}
.content__delivery {
  padding-top: 2rem;
}
.card__delivery {
  justify-content: space-between;
  padding: 1rem;
  display: flex;
  flex-direction: row;
  margin: 1rem;
  border: solid 1px rgba(221, 221, 221, 1);
  border-radius: 10px;
  align-items: center;
}
.card__quantity {
  font-style: normal;
  font-weight: 600;
  font-size: 24px;
  line-height: 33px;
  display: flex;
  align-items: center;
  text-align: center;
  color: #666666;
}

.card__month {
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 33px;
  display: flex;
  align-items: center;
  text-align: center;
  color: #666666;
}

.card__icon {
  margin-right: 0.5rem;
}
</style>
