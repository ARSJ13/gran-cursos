<template>
    <aside>
        <v-container>
         <!-- seta > mdi-apple-keyboard-control -->
            <img class="logo" :src=logo alt="Logo">
            <div class="menu">
                <MenuAside title="apps" icon="mdi-email-outline" subtitle="email"></MenuAside>
                <MenuAside icon="mdi-comment-outline" subtitle="chat"></MenuAside>
                <MenuAside icon="mdi-checkbox-marked-outline" subtitle="Todo"></MenuAside>
                <MenuAside icon="mdi-calendar-outline" subtitle="Calendar"></MenuAside>
            </div>
            <div class="menu">
                <MenuAside
                    title="ui elements"
                    icon="mdi-grid-large"
                    subtitle="grid"
                    span="mdi-apple-keyboard-control"
                    direction="right"
                ></MenuAside>
                <MenuAside icon="mdi-water-outline" subtitle="colors"></MenuAside>
                <MenuAside
                    icon="mdi-credit-card-outline"
                    subtitle="card"
                    span="mdi-apple-keyboard-control"
                    direction="right"
                ></MenuAside>
                <MenuAside icon="mdi-calendar-outline" subtitle="table"></MenuAside>
                <MenuAside
                    icon="mdi-view-grid-outline"
                    subtitle="components"
                    span="mdi-apple-keyboard-control"
                    direction="right"
                ></MenuAside>
            </div>
            <div class="menu">
                <MenuAside
                    title="forms"
                    icon="mdi-checkbox-multiple-blank-outline"
                    subtitle="form elements"
                    span="mdi-apple-keyboard-control"
                    direction="right"
                ></MenuAside>
                <MenuAside icon="mdi-dock-left" subtitle="form layouts"></MenuAside>
                <MenuAside icon="mdi-note-text-outline" subtitle="form wizard"></MenuAside>
                <MenuAside icon="mdi-checkbox-marked-circle-outline" subtitle="form validation"></MenuAside>
            </div>
        </v-container>
    </aside>
</template>

<script>

import MenuAside from './MenuAside'

export default {
  name: 'Menu',
  components: {
    MenuAside
  },
  data(){
    return{
      logo: "logo.png"
    }
  }
}
</script>

<style>
.logo{
  max-width: 10rem;
  width: 100%;
}
.menu{
    margin-bottom: 2.5rem;    
}
</style>