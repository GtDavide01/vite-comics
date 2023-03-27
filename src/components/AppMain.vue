<script>
import AppCards from "./AppCards.vue";
export default {
  name: "AppMain",
  components: {
    AppCards,
  },
  data() {
    return {
      listCards: [
        {
          thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>
<!-- HTML -->
<template>
  <main>
    <div class="containallmain">
      <div class="imgjumbotron">
        <div class="container">
          <div class="current">
            <h2>CURRENT SERIES</h2>
          </div>
        </div>
      </div>
      <div class="contentmenu">
        <div class="container flex-center-column">
          <div class="container-card">
            <AppCards
              v-for="(card, index) in listCards"
              :key="index"
              :img="card.thumb"
              :titolo="card.series"
              :prezzo="card.price"
              :type="card.type"
            />
          </div>
          <div class="leadmore">
            <h2>Load more</h2>
          </div>
        </div>
      </div>
    </div>
    <!-- INFO -->
    <div class="infodcabout">
      <div class="container">
        <ul>
          <li>
            <img
              src="../assets/img/buy-comics-digital-comics.png"
              alt="digital-comics"
            />
            <span>DIGITAL COMICS</span>
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-merchandise.png"
              alt="comics-merchandise"
            />
            <span>DC MERCHANDISE</span>
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-subscriptions.png"
              alt="subscriptionms-comics"
            />
            <span>SUBSCRIPTION</span>
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-shop-locator.png"
              alt="shop-comics"
            />
            <span>COMIC SHOP LOCATOR</span>
          </li>

          <li>
            <img
              src="../assets/img/buy-dc-power-visa.svg"
              alt="dc-power-visa"
            />
            <span>DC POWER VISA</span>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<!-- CSS/SCSS -->
<style lang="scss" scoped>
@use "../../styles/partials/variabili" as *;
.leadmore {
  h2 {
    text-transform: uppercase;
    color: white;
    margin: 20px 0;
    padding: 10px 50px;
    font-size: 20px;
    background-color: #0282f9;
  }
}
.flex-center-column {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.container-card {
  padding: 2rem 0;
  display: flex;
  flex-wrap: wrap;
  margin: 0 auto;
  width: 90%;
}
.containallmain {
  position: relative;
}
.imgjumbotron {
  background-image: url(../assets/img/jumbotron.jpg);
  height: 400px;
  overflow: hidden;

  img {
    width: 100%;
    overflow: hidden;
  }

  .current {
    position: absolute;
    z-index: 999;
    color: white;
    padding: 10px 20px;
    background-color: #0282f9;
    top: 380px;
  }
}

.contentmenu {
  display: flex;
  background-color: #1c1c1c;
  min-height: 150px;
  align-items: center;
}

.infodcabout {
  justify-content: center;
  display: flex;
  align-items: center;
  min-height: 170px;
  background-color: #0282f9;

  ul {
    justify-content: space-between;
    display: flex;
    list-style: none;

    li {
      padding: 0 2rem;
      display: flex;
      align-items: center;

      img {
        width: 50px;
      }

      span {
        color: white;
        padding-left: 1rem;
      }
    }
  }
}
</style>
