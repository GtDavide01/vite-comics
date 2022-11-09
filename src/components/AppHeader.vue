<script>
export default {
  name: "AppHeader",
  data() {
    return {
      listMenu: [
        {
          title: "CHARACTERS",
          href: "/characters",
          active: false,
        },
        {
          title: "COMICS",
          href: "/comics",
          active: true,
        },
        {
          title: "MOVIES",
          href: "/MOVIES",
          active: false,
        },
        {
          title: "TV",
          href: "/tv",
          active: false,
        },
        {
          title: "GAMES",
          href: "/games",
          active: false,
        },
        {
          title: "COLLECTIBLES",
          href: "/collectibles",
          active: false,
        },
        {
          title: "VIDEOS",
          href: "/videos",
          active: false,
        },
        {
          title: "FANS",
          href: "/fans",
          active: false,
        },
        {
          title: "NEWS",
          href: "/news",
          active: false,
        },
        {
          title: "SHOP",
          href: "/shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container">
    <header>
      <div class="logodc">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <div class="menudc">
        <ul>
          <li v-for="(valore, index) in listMenu" :key="index">
            <a :class="{ active: valore.active }" href="{{valore.href}}">{{
              valore.title
            }}</a>
          </li>
        </ul>
      </div>
    </header>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/general.scss" as *;
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 130px;
  .logodc {
    padding: 1rem;
    display: flex;

    width: 30%;
    img {
      max-width: 100%;
    }
  }
  .menudc {
    height: 100%;
    display: flex;
    width: 70%;
    justify-content: end;
    ul {
      align-items: center;
      display: flex;
      list-style: none;
      li {
        display: flex;
        height: 100%;
        align-items: center;
        font-size: 0.8rem;
        line-height: 100%;
        padding: 0 1rem;
        font-weight: 900;
        &:hover,
        &.active {
          border-bottom: 3px solid #0282f9;
          a {
            color: #0282f9;
          }
        }
        a {
          line-height: 100%;
          text-decoration: none;
          color: black;
        }
      }
    }
  }
}
</style>
