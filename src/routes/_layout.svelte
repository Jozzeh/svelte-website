<script>
  import Nav from "../components/Nav.svelte";
  import Footer from "../components/Footer.svelte";

  export let segment;
</script>

<style>
  main {
    position: relative;
    background-color: white;
    margin: 0 auto;
  }

  @media screen and (min-width: 900px) {
    main {
      padding-top: 55px;
    }
  }
</style>

<Nav {segment} />

<main>
  <slot />
</main>

<Footer />
