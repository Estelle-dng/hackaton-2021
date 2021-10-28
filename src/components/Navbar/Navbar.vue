<template>
  <Wrapper>
    <div class="hero"></div>
    <nav class="navbar" id="accueil">
      <div>
        <a href="#accueil">
          <img class="logo" src="../../../public/logo-light.png" alt="logo" />
        </a>
      </div>
      <div>
        <ul>
          <li>
            <a href="#accueil">Accueil</a>
          </li>
          <li>
            <a href="#concept">Notre concept</a>
          </li>
          <li>
            <a href="#about">À propos</a>
          </li>
          <li>
            <Button
            :isRouter="false"
            text="Devenir partenaire"
            ariaLabel="partner"
            link="#partners"
            className="nav-button"
            classA="nav-a"
            />
          </li>
        </ul>
      </div>
    </nav>
  </Wrapper>
</template>

<script>
import Button from "@/components/Button";
import Wrapper from "@/components/Wrapper";

export default {
  name: "Navbar",
  components: { Button, Wrapper },
};
</script>

<style lang="scss">
.hero {
  background: #ccc;
  background: url('../../../public/img/hero.jpg') no-repeat center center;
  background-size: cover;
  box-shadow: 
    inset 0 0 100vw 100vw rgba(0,0,0,0.3),0 16px 8px -8px rgba(0, 0, 0, 0.4);
  width: 100vw;
  height: 100vh;
  top:0;
  left:0;
  position: absolute;
  z-index: -1;
}
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 100px;
  ul{
    justify-content: space-between;
    display: flex;
    li{
      margin-top: 15px;
      margin-left:10px;
      a{color: $ice;}
      &:last-child{
        margin-top: 0;
        }
    }
  }
  .logo {
    width: 100px;
    height: 100px;
    object-fit: contain;
  }
}

@media screen and (max-width: 768px) {
  .navbar {
    padding: 6px 14px 0 14px;
    .logo {
      width: 83px;
    }
  }
}
</style>
