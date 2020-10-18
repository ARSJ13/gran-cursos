<template>
  <main>
    <Header id="header"></Header>
    <Menu id="menu"></Menu>
    <CardsContainer id="cards"></CardsContainer>
    <Footer id="footer"></Footer>
  </main>
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
main{
  display: grid;
  grid-template-rows: 5% 1fr 5%;
  grid-template-columns: 15% 1fr;
  grid-template-areas: 
    "menu header"
    "menu cards"
    "menu footer"
  ;
  gap: 1.5rem;
}
#header{
  grid-area: header;
}
#menu{
  grid-area: menu;
}
#cards{
  grid-area: cards;
  margin: 1rem 0 0 0;
}
#footer{
  grid-area: footer;
}
@media screen and (max-width: 1000px){
  main{
    grid-template-columns: 25%;
  }
}
@media screen and (max-width: 790px){
  main{
    grid-template-columns: 1fr;
    grid-template-areas:
      "header"
      "cards"
      "footer"
    ;
  }
  #header{
    margin:0 1rem 0 0;
  }
  #menu{
    display: none;
  }
  #cards{
    width: 100%;
    margin: 0px auto;
  }
}

</style>