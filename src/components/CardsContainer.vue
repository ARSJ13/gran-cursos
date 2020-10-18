<template>
  <main>
    <header>
      <CardActions></CardActions>
    </header>
    <div class="body-filters">
      <Filters></Filters>
    </div>
    <div class="body-cards">
      <Search></Search>
      <Card
        title="apple watch series 4 gps"
        brand='apple'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to makea type specimen book.'
        rating=34
        price='$399'
        image='watch.jpg'
        alt='Apple Watch'
      ></Card>
      <Card
        title="jbl speaker"
        brand='jbl'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to makea type specimen book.'
        rating=15
        price='$199'
        image='jbl.jpg'
        alt='Jbl Speaker'
      ></Card>
      <Card
        title="apple iphone x 128gb"
        brand='apple'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to makea type specimen book.'
        rating=50
        price='$999'
        image='iphone.jpg'
        alt='Apple Iphone'
      ></Card>
      <Card
        title="beats headphones"
        brand='beats'
        description='Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to makea type specimen book.'
        rating=20
        price='$459'
        image='headphones.jpg'
        alt='Beats Headphones'
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
</style>