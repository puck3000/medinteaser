<template>
  <div class="container">
    <article>
      <h2>
        Ihr neues Gesundheitszentrum beim Bahnhof Biel.
        <span>
          <br />
        </span>
        Ab Oktober 2019.
      </h2>
      <a href="#" target="_blank">Kontakt</a>
      <a href="#" target="_blank">Downloads</a>
    </article>
    <article>
      <h2>
        Französisches Gesundheitszentrum beim Bahnhof Bienne.
        <span>
          <br />
        </span>
        Ab Oktober 2019.
      </h2>
      <a href="#" target="_blank">Contact</a>
      <a href="#" target="_blank">Downloads</a>
    </article>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "home"
};
</script>

<style lang="stylus" scoped>
.container {
  @media screen and (min-width: 768px) {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 2rem;
  }

  article {
    margin-bottom: 3rem;
  }

  h2 {
    margin-bottom: 1rem;

    span {
      display: none;

      @media screen and (min-width: 768px) {
        display: inline;
      }
    }
  }

  a {
    display: block;
  }
}
</style>
