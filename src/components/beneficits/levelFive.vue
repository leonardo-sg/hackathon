<template>
  <div class="card__shape">
    <div class="header__card">
      <span class="title__card">Life</span>
      <span class="points">4500 Pts</span>
    </div>
    <div class="body__card">
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title" style="color:#582D89;"
          ><b>Frete grátis em compras a partir de R$120</b>
        </span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title">Desconto em serviços </span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title" style="color:#582D89;"
          ><b>Brindes exclusivos</b></span
        >
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title">Benefícios em assinatura </span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title" style="color:#582D89;"
          ><b>Mais desconto em produtos selecionados</b>
        </span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title" style="color:#582D89;"
          ><b>Atendimento preferencial</b>
        </span>
      </div>
      <div class="title__line">
        <img class="img__title" :src="icon" alt="" />
        <span class="sub__title">Várias formas de pagamento</span>
      </div>
    </div>
  </div>
</template>

<script>
import Dot from "@/assets/icons/dotPurple.svg";

export default {
  data() {
    return {
      icon: Dot,
    };
  },
};
</script>

<style scoped>
.sub__title {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 22px;
  color: #333333;
  text-align: initial;
}
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
  background-color: #582d89;
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

.points {
  color: #ffffff;
}
</style>
