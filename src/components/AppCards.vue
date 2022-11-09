<script>
export default {
  name: "AppCards",
  props: {
    img: String,
    titolo: String,
    prezzo: String,
    type: String,
  },
  computed: {
    cardShadow() {
      if (this.type === "comic book") {
        return "comic";
      } else {
        return "graphic";
      }
    },
  },
};
</script>

<template>
  <div class="card" :class="cardShadow">
    <div class="img">
      <img :src="img" alt="" />
    </div>
    <div class="titlecard">
      <p>{{ titolo }}</p>
      <span>{{ prezzo }}</span>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  cursor: pointer;
  width: calc(100% / 6 - 20px);
  margin: 30px 10px;
  .img {
    height: 200px;
    overflow: hidden;
    img {
      width: 100%;
    }
  }
  .titlecard {
    p {
      font-size: 0.9rem;
      color: white;
      text-transform: uppercase;
      padding: 10px;
    }
    span {
      color: white;
      padding: 0 10px;
    }
  }
  &.comic {
    box-shadow: 10px 5px 5px #0282f9;
  }
  &.graphic {
    box-shadow: 10px 5px 5px green;
  }
  &:hover {
    transform: scale(1.1);
    transition: 2s;
  }
}
</style>
