<template>
  <header class="header-body">
    <v-container class="header-container">
      <div class="header-items">
        <v-icon color="#0052CC">mdi-checkbox-marked-outline</v-icon>
        <v-icon class="items-icon" color="#0052CC">mdi-comment-outline</v-icon>
        <v-icon class="items-icon" color="#0052CC">mdi-email-outline</v-icon>
        <v-icon class="items-icon" color="#0052CC">mdi-calendar-outline</v-icon>
        <v-icon class="item-opacity" color="#FFAB00">mdi-star</v-icon>
      </div>
      <div class="header-avatar">
        <p>English</p>
        <v-icon class="avatar-icon" color="#0052CC">mdi-bell-outline</v-icon>
        <v-icon color="#0052CC">mdi-magnify</v-icon>
        <div class="avatar">
          <div>
            <h5>John Doe</h5>
            <p>Available</p>
          </div>
          <v-icon class="item-opacity" color="#6554C0" large>mdi-account-circle</v-icon>
        </div>
      </div>
    </v-container>
    <div class="mobile">
      <img class="logo" :src=logo alt="Logo">
      <button><v-icon color="#0052CC" large>mdi-menu</v-icon></button>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data(){
    return{
      logo: 'logo.png'
    }
  }
}
</script>

<style>
.mobile{
  display: none;
}
.header-body{
  width: 100%;
}
.header-container{
  display: flex;
  justify-content: space-between;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  background: #FAFBFC;
}
.header-items{
  display: flex;
  justify-content: center;
  cursor: pointer;
}
.header-items>.items-icon{
  margin: 0 0.5rem;
}
.item-opacity{
  opacity: 0.5;
}
.header-avatar{
  display: flex;
  cursor: pointer;
}
.header-avatar>p{
  align-self: center;
}
.avatar{
  display: flex;
  margin-left: 1rem;
}
.avatar h5{
  color: #6554C0;
}
.avatar-icon{
  margin: 0 0.9rem;
}
@media screen and (max-width: 790px) {
  .mobile{
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-content: center;
    padding: 1rem;
    box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
    background: #FAFBFC;

  }
  .header-container{
    display: none;
  }
}
</style>