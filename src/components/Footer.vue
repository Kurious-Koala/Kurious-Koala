<template>
  <footer class="footer">
    <div class="footer__container">
      <a class="footer__logo" href="#">
        <span class="footer__logo--text footer__logo--text-cursive"
          >kurious</span
        >
        <img
          class="footer__logo--koala"
          alt="logo"
          src="../assets/FooterKoala.png"
        />
        <span class="footer__logo--text footer__logo--text-bold"
          >Koala
          <img
            class="footer__img--leaves"
            alt="leaves"
            src="../assets/FooterLeaves.png"
        /></span>
      </a>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-md-6 col-sm-12 col-xs-12">
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
              class="footer__bottom--bee"
              alt="grass"
              src="../assets/FooterBee.png"
            />
          </section>
        </div>
        <div class="col-lg-4 col-md-12 col-sm-12 col-xs-12">
          <section class="footer__copyright">
            <span> Copyright © 2021 Kurious Koala </span>
          </section>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 col-xs-12">
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
          </section>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  flex: 1 0 auto;
  /* width: auto; */
  color: rgb(22, 21, 21);
  background-color: rgb(150, 209, 155);
  box-shadow: 0 3px 10px rgb(0 0 0 / 0.5);
}

.footer__container {
  width: auto;
  margin: 0 auto;
  /* padding: 40px 0 30px; */
  display: flex;
  flex-direction: column;
  align-items: center;
}

/*** Logo Section ***/
.footer__logo {
  display: flex;
  margin-bottom: 30px;
  flex-direction: column;
  font-size: 20px;
  text-decoration: none;
  color: rgb(22, 21, 21);
}

.footer__logo--koala {
  height: 80px;
  width: 80px;
}

.footer__logo:hover {
  color: #fff;
  transition: ease-in-out 0.3s;
}

.footer__logo--text {
  text-align: center;
  font-size: 1.8em;
  line-height: 2em;
}

.footer__logo--text-cursive {
  font-family: "Henny Penny", cursive;
  font-size: 30px;
}

.footer__logo--text-bold {
  font-size: 30px;
  font-weight: bold;
}

/*** Footer bottom Section ***/
.footer__bottom {
  width: 100%;
}

.footer__img--leaves {
  height: 20px;
  width: 20px;
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

/*** Copyright section ***/

/********** Medium devices only **********/
@media (min-width: 992px) and (max-width: 1199px) {
  .footer__logo--koala {
    height: 70px;
    width: 70px;
  }
  .footer__logo--text,
  .footer__logo--text-cursive {
    font-size: 1em;
  }
}

/********** Small devices only **********/
@media (min-width: 768px) and (max-width: 991px) {
  .footer__logo--koala {
    height: 60px;
    width: 60px;
  }
  .footer__logo--text,
  .footer__logo--text-cursive {
    font-size: 0.8em;
  }
}

/********** Extra small devices only **********/
@media (max-width: 767px) {
  .footer__logo--koala {
    height: 50px;
    width: 50px;
  }
  .footer__logo--text,
  .footer__logo--text-cursive {
    font-size: 0.6em;
  }
  .footer__bottom--bee {
    width: 15px;
    height: 15px;
  }
}
</style>
