<template>
  <div class="MainPage__root">
    <div class="PageImageLeader__root" v-bind:style="{ backgroundImage: 'url(' + landingImg + ')' }">
      <h1 class="PageImageLeader__heading">{{imgHeading}}</h1>
      <p class="PageImageLeader__sub-headline">{{imgSubheadline}}</p>
    </div>
    <div class="ThreePartSection__root PageSection__border">
      <div class="ThreePartSection__part">
        <font-awesome-icon icon="coffee" />
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam lobortis vestibulum ornare. Sed egestas metus et metus auctor pellentesque. Suspendisse.</p>
      </div>
      <div class="ThreePartSection__part">
        <font-awesome-icon icon="coffee" />
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam lobortis vestibulum ornare. Sed egestas metus et metus auctor pellentesque. Suspendisse.</p>
      </div>
      <div class="ThreePartSection__part">
        <font-awesome-icon icon="coffee" />
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam lobortis vestibulum ornare. Sed egestas metus et metus auctor pellentesque. Suspendisse.</p>
      </div>
    </div>
    <div class="MakeCookies__root PageSection__border">
      <h2> Make Some Cookies</h2>
      <div class="ShortDividerLine__root"/>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
      <div class="MakeCookies__info">
        <div>
          <h3>Bake them with friends</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec cursus mi varius, cursus eros vel, pellentesque est. Integer molestie, nibh non commodo ornare, sapien lorem.
          </p>
        </div>
        <img class="MakeCookies__image" v-bind:src="cookiesImg" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      landingImg: '../static/assets/images/aleksander-soroka-1187920-unsplash.jpg',
      imgHeading: 'Starting to Look a lot like Christmas',
      imgSubheadline: 'Let it Snow',
      cookiesImg: '../static/assets/images/mara-conan-233715-unsplash.jpg'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.MainPage__root {
  color: #FD8661;
}

.PageSection__border {
  border-bottom: 1px solid #c4c0c0;
  border-top: 1px solid #c4c0c0;
}

.PageImageLeader__root {
  display: grid;
  grid-template-rows: 50%;
  -webkit-box-sizing: content-box;
  background-color: #FFFFFF;
  background-position: center 100%;
  background-size: cover;
  box-sizing: content-box;
  height: 70vh;
  max-height: 700px;
  min-height: 450px;
  text-align: center;
  text-shadow: 2px 2px #FFFFFF;
}

.PageImageLeader__heading {
  grid-row: 1;
  align-self: end;
  color: #FD8661;
  margin: 0;
}

.PageImageLeader__sub-headline {
  grid-row: 2;
  color: #D50C35;
  font-size: 18px;
  margin: 0;
}

.ThreePartSection__root {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  padding: 80px 0 80px 0;
}

.ThreePartSection__part {
  padding: 20px;
}
.ShortDividerLine__root {
  border-top: 1px solid white;
  margin: 0 auto;
  padding-bottom: 40px;
  width: 80px;
}

.MakeCookies__root {
  background-color: #FE8968;
  color: white;
}

.MakeCookies__info {
  display: grid;
  grid-template-columns: 1fr 1fr;
  justify-items: center;
  padding: 15px;
}

.MakeCookies__image {
  width: 70%;
  padding: 20px;
}
</style>
