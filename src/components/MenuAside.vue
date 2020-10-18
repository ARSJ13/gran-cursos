<template>
  <div class="menu-aside">
    <h4 class="title">{{ title }}</h4>
    <div class="aside-container">
      <div class="aside-content">
        <v-icon class="icon" color="#0052CC">{{ icon }}</v-icon>
        <h4 class="title-icon">{{ subtitle }}</h4>
      </div>
      <div :class=direction>
        <v-icon class="icon-span">{{ span }}</v-icon>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MenuAside",
  props: ['title', 'icon', 'subtitle', 'span', 'direction']
}
</script>

<style>
.menu-aside{
  margin: 1rem 0;
}
.title{
  margin: 1rem 0;
  text-transform: uppercase;
  color: #0052CC;
}
.aside-container{
  display: flex;
  justify-content: space-between;
}
.aside-content{
  display: flex;
  align-items: center;
}
.aside-content>.icon{
  color: #172B4D;
  margin-right: 0.7rem;
  cursor: pointer;
}
.aside-content>.title-icon{
  color: #091E42;
  text-transform: capitalize;
}
.right{
  transform: rotate(90deg);
}
.bottom{
  transform: rotate(-180deg);
}


</style>