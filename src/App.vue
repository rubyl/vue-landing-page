<template>
    <div id="app">
        <!-- <div id="header-nav" class="nav-bars">
            <router-link to="/">Home</router-link> |
        </div> -->
        <router-view/>
    </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      wordCount: 0,
      latestWord: 'Latest_Word'
    }
  }
}
</script>

<style lang="scss">

  body {
    margin: 0;
  }

    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;

        .nav-bars{
            background: cornflowerblue;
            padding: 10px;
            color: white;
            a {
                color: white;
                text-decoration: none;
            }
        }
    }
</style>
