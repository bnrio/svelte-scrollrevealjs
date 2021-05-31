<script>
  export let name;
  import { onMount } from "svelte";
  import ScrollReveal from "scrollreveal";

  onMount(() => {
    ScrollReveal.debug = true;
    ScrollReveal().reveal(".box", {
      easing: "cubic-bezier(0.5, 0, 0, 1)",
      cleanup: true,
      delay: 100
    });
  });
</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  .box {
    width: 50%;
    margin: 30px auto;
    background: beige;
    padding: 200px 0;
    height: calc(100vh - 400px);
    -webkit-border-radius: 20px;
    -moz-border-radius: 20px;
    border-radius: 20px;
  }

  .box-2 {
    background: cadetblue;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<main>

  <div class="box">Box 1</div>
  <div class="box box-2">Box 2</div>
  <div class="box">Box 1</div>
  <div class="box box-2">Box 2</div>
  <div class="box">Box 1</div>
  <div class="box box-2">Box 2</div>
  <div class="box">Box 1</div>
  <div class="box box-2">Box 2</div>
  <div class="box">Box 1</div>
  <div class="box box-2">Box 2</div>
  <div class="box">Box 1</div>
  <div class="box box-2">Box 2</div>

</main>
