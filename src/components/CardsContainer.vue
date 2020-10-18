<template>
  <main class="cards-container">
    <header class="card-actions">
      <CardActions></CardActions>
    </header>
    <div class="body-filters">
      <Filters></Filters>
    </div>
    <div class="body-cards">
      <Search class="card-search"></Search>
      <Card
        title="apple watch series 4 gps"
        brand='apple'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s.'
        rating=34
        price='$399'
        image='watch.jpg'
        alt='Apple Watch'
      ></Card>
      <Card
        title="jbl speaker"
        brand='jbl'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s.'
        rating=15
        price='$199'
        image='jbl.jpg'
        alt='Jbl Speaker'
      ></Card>
      <Card
        title="apple iphone x 128gb"
        brand='apple'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s.'
        rating=50
        price='$999'
        image='iphone.jpg'
        alt='Apple Iphone'
      ></Card>
      <Card
        title="beats headphones"
        brand='beats'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s.'
        rating=20
        price='$459'
        image='headphones.jpg'
        alt='Beats Headphones'
      ></Card>
      <Card
        title="apple watch series 4 gps"
        brand='apple'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s.'
        rating=34
        price='$399'
        image='watch.jpg'
        alt='Apple Watch'
      ></Card>
      <Card
        title="jbl speaker"
        brand='jbl'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s.'
        rating=15
        price='$199'
        image='jbl.jpg'
        alt='Jbl Speaker'
      ></Card>
      <Card
        title="apple iphone x 128gb"
        brand='apple'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s.'
        rating=50
        price='$999'
        image='iphone.jpg'
        alt='Apple Iphone'
      ></Card>
    </div>
  </main>
</template>

<script>
import CardActions from './CardActions'
import Filters from './Filters'
import Search from './Search'
import Card from './Card'

export default {
  name: 'CardsContainer',
  components: {
    CardActions,
    Filters,
    Search,
    Card
  }
}
</script>

<style>
.cards-container{
  display: grid;
  grid-template-rows: 3% 1fr;
  grid-template-columns: 25% 1fr;
  grid-template-areas:
    "header header"
    "filters cards"
  ;
  gap: 1rem;
  margin-bottom: 1rem;
}
header{
  grid-area: header;
}
.body-filters{
  grid-area: filters;
}
.body-cards{
  grid-area: cards;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
}
@media screen and (max-width: 1000px) {
  .body-filters{
    display: none;
  }
  .cards-container{
  display: grid;
  grid-template-rows: 1fr;
  grid-template-columns: 1fr;
  grid-template-areas:
    "header"
    "cards"
  ;
  gap: 0;
  }
  .card-actions{
    width: 96%;
    margin: 0 auto;
  }
  .card-search{
    width: 96%;
    margin: 0 auto;
  }
}
</style>