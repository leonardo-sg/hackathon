<template>
  <div>
    <div class="points__section">
      <div class="image__icon">
        <img :src="icon" alt="" />
      </div>
      <div class="content__card">
        <div class="title">Você está no nível</div>
        <div class="sub__title">
          Alcance o nível 3 acumulando mais 350 pontos.
        </div>
        <div class="info__points">
          <img class="icon__about" :src="iconArrow" alt="" />
          <div class="info__card">
            No fim do mês, 60 pontos expiram. Por que acontece isso?
          </div>
        </div>
      </div>
    </div>
    <div class="card__points">
      <LevelOne />
      <br />
      <LevelTwo />
      <br />
      <LevelTree />
      <br />
      <LevelFour />
    </div>
  </div>
</template>

<script>
import Points from "@/assets/icons/pointsGroup.png";
import ArrowD from "@/assets/icons/arrowD.svg";
import LevelOne from "../components/beneficits/levelOne.vue";
import LevelTwo from "../components/beneficits/levelTwo.vue";
import LevelTree from "../components/beneficits/levelTree.vue";
import LevelFour from "../components/beneficits/levelFour.vue";

export default {
  name: "About",
  components: { LevelOne, LevelTwo, LevelTree, LevelFour },
  data() {
    return {
      icon: Points,
      iconArrow: ArrowD,
    };
  },
};
</script>

<style scoped>
.points__section {
  background-color: #ffffff;
  padding: 2rem;
  display: flex;
  flex-direction: row;
}
.content__card {
  display: flex;
  flex-direction: column;
}

.title {
  text-align: initial;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 25px;
  color: #333333;
}
.sub__title {
  text-align: initial;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 16px;
  color: #666666;
}

.info__card {
  text-align: initial;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 14px;
  color: #666666;
}

.image__icon {
  margin-right: 0.5rem;
}

.info__points {
  display: flex;
  flex-direction: row;
}

.icon__about {
  margin-right: 0.5rem;
}
.card__points {
  padding: 2rem;
}
</style>
