<template>
  <section class="search-container">
    <div class="search-header">
      <div class="search-results">
        <h4>7,618 results found in 5ms</h4>
      </div>
      <div class="search-nav">
        <button>Default<v-icon class="search-icon">mdi-chevron-right</v-icon></button>
        <button><v-icon color="#0052CC">mdi-view-grid-outline</v-icon></button>
        <button><v-icon color="#0052CC">mdi-menu</v-icon></button>
      </div>
    </div>
    <div class="search-body">
      <input type="search" placeholder="Search hear">
      <button><v-icon>mdi-magnify</v-icon></button>
    </div>
  </section>
</template>

<script>
export default {
  name: "Search"

}
</script>

<style>
.search-header{
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.search-results>h4{
  font-weight: 400;
}
.search-nav{
  font-size: 0.8rem;
}
.search-nav>button{
  padding: 0.5rem;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
  margin-left: 0.5rem;
  color: #0052CC;
  font-weight: 600;
}
.search-icon{
  margin-left: 1.5rem;
  transform: rotate(90deg);
}
.search-body{
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
  margin: 1rem 0;
  padding: 0.5rem 1rem;
  display: flex;
  justify-content: space-between;
}
@media screen and (max-width: 580px) {
  .search-header{
    display: none;
  }
}

</style>