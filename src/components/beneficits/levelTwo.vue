<template>
  <div class="card__shape">
    <div class="header__card">
      <span class="title__card">Nível 3</span>
      <img class="icon__point" :src="iconCheck" alt="" />
    </div>
    <div class="body__card">
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span>Lorem ipsum dolor sit amet </span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span>Consectetur adipiscing elit</span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span>Praesent id tincidunt augue</span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span><b>Nullam suscipit a nisi</b></span>
      </div>
    </div>
  </div>
</template>

<script>
import Dot from "@/assets/icons/dotGreen.svg";
import check from "@/assets/icons/levelTwo.svg";
export default {
  name: "levelTwo",
  data() {
    return {
      icon: Dot,
      iconCheck: check,
    };
  },
};
</script>

<style scoped>
.title__card {
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 25px;
  color: #ffffff;
}

.icon__point {
  width: 32px;
}
.card__shape {
  border: 1px solid rgba(221, 221, 221, 1);
  border-radius: 10px;
  background-color: #ffffff;
}
.header__card {
  border-radius: 10px 10px 0 0;
  align-items: center;
  height: 49px;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  background-color: rgba(123, 207, 157, 1);
}
.title__line {
  display: flex;
  flex-direction: row;
}
.img__title {
  margin-right: 1rem;
}
.body__card {
  padding: 1rem;
}
</style>
