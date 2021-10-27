<template>
  <footer class="footer">
    <div class="footer_container">
      <a class="footer-logo" href="#">
        <span class="footer-logo_text footer-logo_text-cursive">Kurious</span>
        <span class="footer-logo_text footer-logo_text-bold">Koala</span>
      </a>
      <div class="footer_nav">
        <ul class="footer-nav_list">
          <li class="footer-nav_item">
            <a class="footer-nav_link" href="#">About</a>
          </li>
          <li class="footer-nav_item">
            <a class="footer-nav_link" href="#">Login</a>
          </li>
          <li class="footer-nav_item">
            <a class="footer-nav_link" href="#">Contact</a>
          </li>
        </ul>
      </div>
      <address class="footer_copyright">Copyright © 2021 Kurious Koala</address>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  color: rgb(22, 21, 21);
  background-color: rgb(150, 209, 155);
}

.footer_container {
  width: 80%;
  margin: 0 auto;
  padding: 80px 0 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.footer-logo {
  display: flex;
  margin-bottom: 30px;
  flex-direction: column;
  font-size: 20px;
  text-decoration: none;
  color: rgb(22, 21, 21);
}

.footer-logo:hover {
  color: #fff;
  transition: ease-in-out 0.3s;
}

.footer-logo_text {
  text-align: center;
  font-size: 1.8em;
  line-height: 1em;
  z-index: 5;
}

.footer-logo_text-cursive {
  font-family: "Dancing Script", cursive;
  text-transform: lowercase;
  font-weight: bold;
}

.footer-logo_text-bold {
  text-transform: uppercase;
}

.footer_copyright {
  margin: 40px auto;
  margin-bottom: 30px;
  padding: 0;
  font-style: normal;
}

.footer-nav_list {
  margin: 0;
  padding: 0;
  min-width: 50%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  list-style: none;
}

.footer-nav_item {
  margin: 0 15px;
  padding: 0;
}

.footer-nav_link {
  display: block;
  font-size: 1em;
  text-transform: uppercase;
  text-decoration: none;
  color: rgb(22, 21, 21);;
}

.footer-nav_link:hover,
.footer-nav_link:focus {
  color: #fff;
  transition: ease-in-out 0.3s;
}
</style>
