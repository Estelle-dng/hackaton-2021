<template>
  <Wrapper>
    <nav class="navbar">
      <div>
        <a href="#accueil">
          <img class="logo" src="../../../public/logo.png" alt="logo" />
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
            link="#partner"
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
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-top: 24px;
  ul{
    justify-content: space-between;
    display: flex;
    li{
      margin-top: 15px;
      margin-left:10px;
      &:last-child{margin-top: 0;}
      .nav-button {
        line-height: 15px;
        background-color: $ice;
        border: 1px solid $purple;
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
