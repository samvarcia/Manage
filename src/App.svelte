<script>
  import Header from "./components/Header.svelte";
  import Hero from "./components/Hero.svelte";
  import Facts from "./components/Facts.svelte";
  import Users from "./components/Users.svelte";
  import Banner from "./components/Banner.svelte";
  import Footer from "./components/Footer.svelte";
</script>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Be+Vietnam:wght@400;500;700&display=swap");
  :global(:root) {
    --main-orange: hsl(12, 88%, 59%);
    --main-gray: #9d9ea2;
    --container: 20px 100px;
  }

  :global(body) {
    background-color: #fafafa;
    color: hsl(228, 39%, 23%);
    margin: 0;
    padding: 0;
    font-family: "Be Vietnam", sans-serif;
    overflow-x: hidden !important;
  }
</style>

<main>
  <Header />
  <Hero />
  <Facts />
  <Users />
  <Banner />
  <Footer />
</main>
