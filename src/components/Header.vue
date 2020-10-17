<template>
  <header>
    <v-container class="header-container">
      <div class="header-items">
        <v-icon>mdi-checkbox-marked-outline</v-icon>
        <v-icon class="items-icon">mdi-comment-outline</v-icon>
        <v-icon class="items-icon">mdi-email-outline</v-icon>
        <v-icon class="items-icon">mdi-calendar-outline</v-icon>
        <v-icon class="item-opacity">mdi-star-outline</v-icon>
      </div>
      <div class="header-avatar">
        <p>English</p>
        <v-icon class="avatar-icon">mdi-bell-outline</v-icon>
        <v-icon >mdi-magnify</v-icon>
        <div class="avatar">
          <div>
            <h5>John Doe</h5>
            <p>Available</p>
          </div>
          <v-icon class="item-opacity" large>mdi-account-circle</v-icon>
        </div>
      </div>
    </v-container>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style>
header{
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
}
.header-container{
  display: flex;
  justify-content: space-between;
}
.header-items{
  display: flex;
  justify-content: center;
}
.header-items>.items-icon{
  margin: 0 0.5rem;
}
.item-opacity{
  opacity: 0.5;
}
.header-avatar{
  display: flex;
}
.header-avatar>p{
  align-self: center;
}
.avatar{
  display: flex;
  margin-left: 1rem;
}
.avatar-icon{
  margin: 0 0.9rem;
}
</style>