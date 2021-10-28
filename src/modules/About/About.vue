<template>
  <div id="about" class="about">
    <Wrapper>
     <div class="wrapper">

      <div class="a">
        <p class="title">Notre<br/>Philosophie<br/>Culturelle et<br/>Artistique</p>
      </div>
      
      <div class="b line">
        <strong>
          <ul>
            <li>Anouck</li>
            <li>Clara</li>
            <li>Corentin</li>
            <li>Erwann</li>
            <li>Estelle</li>
            <li>Jeanne</li>
            <li>Julia</li>
            <li>Julien</li>
          </ul>
        </strong>
      </div>

      <div class="c line">
        <p>Pourquoi Mosaë</p>
      </div>

      <div class="f line">
        <p>Notre envie était de rendre facilement accessible à tous toutes les formes d'arts, de culture ou d'évènements se déroulant dans notre ville de manière hebdomadaire</p>
        <br><br>
        <p>Après avoir consulté notre entourage et des professionnels du milieu, nous avons constaté le manque de mise en avant de certains artistes au profit des "best sellers" ce qui tue la diversité.</p>
        <br><br>
        <p>Nous avons donc voulu créer une plateforme où chacun pourrait participer et signaler un évènement près de chez lui.</p>
        <br><br>
        <h6>C'est ainsi qu'est né Mosaë</h6>
      </div>

    </div>
    </Wrapper>
  </div>
</template>

<script>
import Wrapper from '@/components/Wrapper';
export default {
  name: "About",
  components:{ Wrapper}
};
</script>

<style lang="scss" scoped>
.about{
  padding-top: 100px;
  padding-bottom: 100px;
  background-color: $yellow;
  background-image: url("https://www.transparenttextures.com/patterns/asfalt-dark.png");
}
.line {
    border-top: 3px solid #000;
    padding: 20px 0px 20px 0px;
}
.wrapper {
    display: grid;
    grid-template-columns: 50% 2% 50%;
    grid-template-rows: auto;
    width: 80%;
    margin: 50px auto;
}
.title {
    font-size: 3em;
    line-height: 1em;
    font-family: futura-pt-bold, sans-serif;
    padding-bottom: 20px;
}
.b ul {
    list-style: none;
}
.a {
    /*   or grid-area: row-start / col start / row end / col end */
    
    grid-column: 1 / 2;
    grid-row: 1 / 2;
}
.b {
    grid-column: 3 / 4;
    grid-row: 1 / 2;
}
.c {
    font-weight: bold;
    font-size: 1.7em;
    grid-column: 1 / 2;
    grid-row: 2 / 3;
}
.d {
    font-weight: bold;
    font-size: 1.7em;
    grid-column: 1 / 2;
    grid-row: 3 / 4;
}
.e {
    font-weight: bold;
    font-size: 1.7em;
    grid-column: 1 / 2;
    grid-row: 4 / 5;
}
.f {
    grid-column: 3 / 4;
    grid-row: 2 / 3;
}
.g {
    grid-column: 3 / 4;
    grid-row: 3 / 4;
}
.h {
    grid-column: 3 / 4;
    grid-row: 4 / 5;
}

/* ========================================== MEDIA QUERIES ===================== */

@media only screen and (min-width: 460px) {
    .wrapper {
        display: grid;
        grid-template-columns: auto;
        grid-template-rows: auto;
    }
    .a {
   
        
        grid-row: 1 / 2;
    }
    .b {
        grid-column: 1 /2;
        grid-row: 2 / 3;
    }
    .c {
        grid-row: 3 / 4;
    }
    .d {
        grid-row: 4 / 5;
    }
    .e {
        grid-row: 5 / 6;
    }
    .f {
        grid-column: 1 /2;
        grid-row: 6 / 7;
    }
    .g {
        grid-column: 1 /2;
        grid-row: 8 / 9;
    }
    .h {
        grid-column: 1 /2;
        grid-row: 9 / 10;
    }
}

@media only screen and (min-width: 850px) {
    .wrapper {
    display: grid;
    grid-template-columns: 50% 2% 50%;
    grid-template-rows: auto;
    }
.a {
    /*   or grid-area: row-start / col start / row end / col end */
    
    grid-column: 1 / 2;
    grid-row: 1 / 2;
}
.b {
    grid-column: 3 / 4;
    grid-row: 1 / 2;
}
.c {
    font-weight: bold;
    font-size: 1.7em;
    grid-column: 1 / 2;
    grid-row: 2 / 3;
}
.d {
    font-weight: bold;
    font-size: 1.7em;
    grid-column: 1 / 2;
    grid-row: 3 / 4;
}
.e {
    font-weight: bold;
    font-size: 1.7em;
    grid-column: 1 / 2;
    grid-row: 4 / 5;
}
.f {
    grid-column: 3 / 4;
    grid-row: 2 / 3;
}
.g {
    grid-column: 3 / 4;
    grid-row: 3 / 4;
}
.h {
    grid-column: 3 / 4;
    grid-row: 4 / 5;
}
}
</style>
