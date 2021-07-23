<template>
  <div class="content__delivery">
    <div class="card__delivery">
      <div class="card__content">
        <div class="card__calendar">
          <span class="card__quantity">12</span>
          <span class="card__month">Set</span>
        </div>
        <div>
          <img class="card__icon" :src="iconColeira" />
        </div>
      </div>
      <div>
        <img :src="iconPontos" />
      </div>
    </div>
  </div>
</template>

<script>
import Coleira from "@/assets/icons/coleira.svg";
import Pts from "@/assets/icons/pts.svg";

export default {
  name: "newDeliveryTwo",
  data() {
    return {
      iconColeira: Coleira,
      iconPontos: Pts,
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
.card__content {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.card__calendar {
  margin-right: 2rem;
}
</style>
