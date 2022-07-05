<template>
  <div id="app">
   <MainHeader>

   </MainHeader>
    <router-view/>
  </div>
</template>

<script>
    import MainHeader  from "./components/MainHeader"
    export default {
        name: 'App',
        components: {
            MainHeader
        }
    }
</script>

<style lang="scss">
#app {
  color: #ff8080;
  text-align: center;
  font-family: "Times New Roman";
}

nav {
  padding: 40px;

  a {
    font-weight: normal;
     color: #ff8080;

    &.router-link-exact-active {
      color: #ff0000;
    }
  }
}
li {
    margin-left: 20px;
    list-style-type: none;
}
p {
   margin-left: 20px;
   max-width: 600px;
}
</style>
