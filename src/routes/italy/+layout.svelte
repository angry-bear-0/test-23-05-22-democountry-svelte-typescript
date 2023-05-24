<script>
  import Container from "../../components/Container.svelte";
  import Header from "../../components/Header.svelte";
  import Footer from "../../components/Footer.svelte";
  import Banner from "../../components/Banner.svelte";
  import SideBar from "../../components/SideBar.svelte";
</script>

<Container>
  <Header/>
  <Banner/>
  <div class="flex items-center">
    <SideBar/>
  </div>

  <slot/>

  <Footer/>
</Container>