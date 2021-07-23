<template>
  <div class="card">
    <a-card hoverable class="card__shape">
      <div class="card__container">
        <div class="avartar__img">
          <img :src="avatarIcon" alt="" />
        </div>
        <div class="card__content">
          <span class="avatar__title">
            Você está no
          </span>
          <span class="avatar__content">
            Puppy
          </span>
        </div>
        <div>
          <img class="arrow__act" :src="arrowIcon" @click="open" alt="" />
        </div>
      </div>
    </a-card>
    <div class="footer__card">
      <img style="width:100%;" :src="icon" alt="" />
    </div>
  </div>
</template>

<script>
import avatar from "../../assets/icons/Group.svg";
import arrow from "../../assets/icons/arrow_right.svg";
import fire from "../../assets/icons/fire.svg";

export default {
  name: "CardClient",
  data() {
    return {
      avatarIcon: avatar,
      arrowIcon: arrow,
      icon: fire,
    };
  },
  methods: {
    open() {
      console.log("teste");
      this.$router.push("/about");
    },
  },
};
</script>

<style scoped>
.card {
  border: 1px solid rgba(196, 196, 196, 1);
  border-radius: 0.625rem;
}
.card__shape {
  border-radius: 0.625rem 0.625rem 0 0;
  width: 19.75rem;
  height: 7rem;
}

.card__avatar {
  width: 4rem;
  height: 4rem;
}
.card__description {
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 33px;
  color: #333333;
}

.card__container {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}
.card__content {
  display: flex;
  flex-direction: column;
}
.avartar__img {
  padding-right: 1rem;
}
.avatar__title {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 19px;
  color: #666666;
}
.avatar__content {
  font-style: normal;
  font-weight: bold;
  font-size: 1.5rem;
  line-height: 2.063rem;
  color: #333333;
}

.footer__card {
  display: flex;
  background-color: #f8f8f8;
  width: 19.75rem;
  justify-content: center;
  align-items: center;
}

.arrow__act {
  cursor: pointer;
}
</style>
