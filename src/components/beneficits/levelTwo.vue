<template>
  <div class="card__shape">
    <div class="header__card">
      <span class="title__card">Young</span>
      <span class="points" style="color:#ffffff;">300 Pts</span>
    </div>
    <div class="body__card">
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title">Desconto em serviços</span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title" style="color:#28C291;"
          ><b>Mais desconto em produtos selecionados</b>
        </span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title">Benefícios em assinatura</span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title">Várias formas de pagamento</span>
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

.sub__title {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 22px;
  color: #333333;
  text-align: initial;
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
