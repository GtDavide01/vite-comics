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
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>

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

<style lang="scss" scoped>
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
