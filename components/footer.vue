<template>
  <div class="footer">
    <div class="iconmain">
      <v-icon class="icon" style="color: gray"
        >mdi-account-supervisor-circle</v-icon
      >
      <v-icon class="icon" style="color: gray">mdi-instagram </v-icon>
      <v-icon class="icon" style="color: gray">mdi-whatsapp</v-icon>
      <v-icon class="icon" style="color: gray">mdi-email</v-icon>
    </div>
    <div class="anchor">
      <a href=""> <span style="color: gray">Home</span></a>
      <a href=""><span style="color: gray">Destinations</span></a>
      <a href=""><span style="color: gray">Contacts</span></a>
    </div>
    <br />
    <div>
      <span>© 2021 Nusa Penida Tourism Board All Rights Reserved</span>
      <br />
      <span>Klungkung Regency</span>
      <br />
      <span>Nusa Penida, Bali - Indonesia</span>
      <br />

      <span style="font-size: 60%">Powered by JanuMedia with NuxtJS</span>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.footer {
  background-color: black;
  height: 100%;
  width: 100%;
  text-align: center;
  margin-top: 5%;
}
a {
  text-decoration: none;
  color: gray;
}
span {
  padding: 1%;
  color: gray;
  font-size: 80%;
  color: white;
}
.icon {
  padding: 1%;
}
</style>