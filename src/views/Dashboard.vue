<template>
  <v-container>
    <Header></Header>
    <Menu></Menu>
    <CardsContainer></CardsContainer>
    <Footer></Footer>
  </v-container>
</template>

<script>

  import Header from '../components/Header'
  import Menu from '../components/Menu'
  import CardsContainer from '../components/CardsContainer'
  import Footer from '../components/Footer'

export default {
  name: "Dashboard",
  components: {
    Header,
    Menu,
    CardsContainer,
    Footer
  }

}
</script>

<style>

</style>