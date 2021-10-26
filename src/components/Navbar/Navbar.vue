<template>
  <nav class="navbar">
    <div>
      <a href="#">
        <img
          class="logo"
          src="@/assets/logo.png"
          alt="logo"
        />
      </a>
    </div>
    <div>
      <Button
        :isRouter="false"
        text="CTA"
        ariaLabel="CTA"
        link="#"
        className="nav-button"
        classA="nav-a"
      />
    </div>
  </nav>
</template>

<script>
import Button from "@/components/Button";

export default {
  name: "Navbar",
  components: { Button },
};
</script>

<style lang="scss">
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-top: 24px;
  .nav-button {
    background-color: beige;
    border: 1px solid rgb(57, 56, 151);
    @media (max-width: 500px) {
      display: none;
    }
    .nav-a {
      color: rgb(57, 56, 151);
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
