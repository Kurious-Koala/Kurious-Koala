<template>
<!-- Footer Logo -->
  <footer class="footer">
    <div class="footer__container">
      <span
        class="footer__logo--text footer__logo--text-cursive"
        :style="{ color: black }"
        >kurious</span
      >
      <img
        class="footer__logo--koala"
        alt="logo"
        src="../assets/FooterKoala.png"
      />
      <span
        class="footer__logo--text footer__logo--text-bold"
        :style="{ color: black }"
        >Koala
        <img
          class="footer__img--leaves"
          alt="leaves"
          src="../assets/FooterLeaves.png"
      /></span>
    </div>
    <!-- Images -->
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-md-6 col-sm-6 col-xs-6">
          <section class="footer__bottom">
            <img
              class="footer__bottom--grass hidden-xs hidden-sm"
              alt="grass"
              src="../assets/FooterGrass.png"
            />
            <img
              class="footer__bottom--grass hidden-xs hidden-sm"
              alt="grass"
              src="../assets/FooterGrass.png"
            />
            <img
              class="footer__bottom--firstTree hidden-sm"
              alt="tree"
              src="../assets/FooterTree.png"
            />
            <img
              class="footer__bottom--secondTree hidden-sm"
              alt="tree"
              src="../assets/FooterTree.png"
            />
            <img
              class="footer__bottom--flowers hidden-xs hidden-sm"
              alt="flowers"
              src="../assets/FooterFlowers.png"
            />
            <img
              class="footer__bottom--flowers hidden-xs hidden-sm"
              alt="flowers"
              src="../assets/FooterFlowers.png"
            />
            <img
              class="footer__bottom--bee"
              alt="bee"
              src="../assets/FooterBee.png"
            />
          </section>
        </div>
        <!-- Copyright -->
        <div class="col-lg-4 col-md-12 col-sm-6 col-xs-6">
          <section class="footer__copyright">
            <span> Copyright © 2021 Kurious Koala </span>
          </section>
        </div>
        <!-- Images --> 
        <div class="col-lg-4 col-md-6 col-sm-6 col-xs-12">
          <section class="footer__bottom">
            <img
              class="footer__bottom--grass hidden-xs hidden-sm"
              alt="grass"
              src="../assets/FooterGrass.png"
            />
            <img
              class="footer__bottom--firstTree hidden-xs hidden-sm"
              alt="grass"
              src="../assets/FooterTree.png"
            />
            <img
              class="footer__bottom--secondTree hidden-xs hidden-sm"
              alt="grass"
              src="../assets/FooterTree.png"
            />
            <img
              class="footer__bottom--grass hidden-xs hidden-sm"
              alt="grass"
              src="../assets/FooterGrass.png"
            />
            <img
              class="footer__bottom--flowers hidden-xs hidden-sm"
              alt="flowers"
              src="../assets/FooterFlowers.png"
            />
            <img
              class="footer__bottom--grass hidden-xs hidden-sm"
              alt="grass"
              src="../assets/FooterGrass.png"
            />
          </section>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      black: "#000000",
      lightGreen: "#96d19b",
    };
  },
};
</script>

<style scoped>
/*** Footer Background ***/
.footer {
  background: #00F260;  /* fallback for old browsers */
  background: -webkit-linear-gradient(to bottom, #81cff0, #7ddfa4);  /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to bottom, #03b3ff, #00F260); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}

.footer__container {
  width: auto;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 20px;
}

/*** Logo Section ***/
.footer__logo {
  display: flex;
  margin-bottom: 30px;
  flex-direction: column;
  font-size: 20px;
  text-decoration: none;
}

.footer__logo--koala {
  height: 60px;
  width: 60px;
}

.footer__logo:hover {
  transition: ease-in-out 0.3s;
}

.footer__logo--text-cursive {
  font-size: 1em;
  font-family: "Henny Penny", cursive;
  line-height: 2.2em;
}

.footer__logo--text-bold {
  font-size: 1em;
  font-weight: bold;
  padding-left: 10px;
}

/*** Footer bottom Section(images) ***/
.footer__bottom {
  width: 100%;
}

.footer__img--leaves {
  height: 13px;
  width: 13px;
  margin-bottom: 5px;
}

.footer__bottom--grass {
  width: 20px;
  height: 20px;
  margin-right: 20px;
  position: relative;
  bottom: -25px;
}

.footer__bottom--firstTree {
  width: 70px;
  height: 70px;
  margin-right: -15px;
}

.footer__bottom--secondTree {
  width: 60px;
  height: 60px;
  margin-right: 30px;
  position: relative;
  bottom: -5px;
}

.footer__bottom--bee {
  position: absolute;
  bottom: 0;
  right: 0;
  width: 20px;
  height: 20px;
  position: relative;
  top: -70px;
  right: -30px;
}

.footer__bottom--flowers {
  width: 25px;
  height: 25px;
  position: relative;
  bottom: -23px;
}

/*** Copyright section ***/
.footer__copyright {
  margin-top: 40px;
  font-size: 0.8em;
}

/********** Medium devices only **********/
@media (min-width: 992px) and (max-width: 1199px) {
  .footer__logo--koala {
    height: 50px;
    width: 50px;
  }
  .footer__logo--text,
  .footer__logo--text-cursive {
    font-size: 1em;
  }
  .footer__bottom--grass {
    position: relative;
    bottom: -45px;
  }
  .footer__bottom--firstTree {
    position: relative;
    bottom: -20px;
  }
  .footer__bottom--secondTree {
    position: relative;
    bottom: 10px;
  }
  .footer__bottom--secondTree {
    position: relative;
    bottom: -25px;
  }
  .footer__bottom--flowers {
    position: relative;
    bottom: -43px;
  }
  .footer__img--leaves {
    height: 9px;
    width: 9px;
  }
  .footer__copyright {
    margin-top: 65px;
    font-size: 0.6em;
  }
}

/********** Small devices only **********/
@media (min-width: 768px) and (max-width: 991px) {
  .footer__logo--koala {
    height: 40px;
    width: 40px;
  }
  .footer__logo--text,
  .footer__logo--text-cursive {
    font-size: 0.6em;
  }
  .footer__bottom--grass {
    position: relative;
    bottom: -45px;
  }
  .footer__bottom--firstTree {
    position: relative;
    bottom: -20px;
  }
  .footer__bottom--secondTree {
    position: relative;
    bottom: 10px;
  }
  .footer__bottom--secondTree {
    position: relative;
    bottom: -25px;
  }
  .footer__bottom--flowers {
    position: relative;
    bottom: -43px;
  }
  .footer__img--leaves {
    height: 8px;
    width: 8px;
  }
  .footer__copyright {
    margin-bottom: 15px;
    font-size: 0.5em;
  }
}

/********** Extra small devices only **********/
@media (max-width: 767px) {
  .footer__logo--koala {
    height: 45px;
    width: 45px;
  }
  .footer__logo--text,
  .footer__logo--text-cursive {
    font-size: 0.6em;
  }
  .footer__bottom--bee {
    width: 15px;
    height: 15px;
    position: relative;
    top: 10px;
  }
  .footer__img--leaves {
    height: 8px;
    width: 8px;
  }
  .footer__copyright {
    margin-top: 50px;
    font-size: 0.4em;
  }
}
</style>
