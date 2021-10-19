<template>
  <div class="footer">
    <div class="social-network">
      <ul>
        <li>
            <h1>Connected with us on social networks!</h1>
        </li>
        <li>
          <a href=""><img alt="linkedin" src="../assets/linkedin.svg" /></a>
        </li>
        <li>
          <a href=""><img alt="twitter" src="../assets/twitter.svg" /></a>
        </li>
        <li>
          <a href=""><img alt="instagram" src="../assets/instagram.svg" /></a>
        </li>
        <li>
          <a href=""><img alt="facebook" src="../assets/facebook.svg" /></a>
        </li>
      </ul>
    </div>
    <div class="copyright">
      <p>Copyright © 2021 Online Game</p>
    </div>
  </div>
</template>

<style scoped>
.footer {
  background-color: #ebdede;
  display: flex;
  height: 30vh;
  justify-content: right;
  align-items: flex-end;
}
h1 {
  font-family: Ribeye;
  padding-bottom: 50px;
  font-size: medium;
}
.footer p {
  font-family: Roboto;
  padding-top: 40px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
.copyright {
  display: flex;
  height: 30vh;
  justify-content: center;
  align-items: flex-end;
  margin-top: 50px;
}
</style>
