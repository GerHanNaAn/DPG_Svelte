<script>
  import OneScquare from "./OneScquare.svelte";
  import ThreeScquares from "./ThreeScquares.svelte";
</script>

<style>
  main {
    background: url(./cat.jpg);
    background-size: cover;
    background-position: center;
    min-height: 100vh;
  }
  .container {
    padding: 50px 0;
    max-width: 976px;
    height: 100%;
    margin: 0 auto;
    background: hsla(56, 39%, 72%, 0.616);
  }
  .row {
    display: flex;
  }
</style>

<main>
  <div class="container">
    <div class="row">
      <OneScquare />
      <ThreeScquares />
    </div>
  </div>
</main>
