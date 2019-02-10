<template>
  <f7-app :params="f7params">
    <f7-statusbar></f7-statusbar>
    <!-- initial page is specified in routes.js -->
    <f7-view main url="/" />
  </f7-app>
</template>

<script>
import HomePage from './components/HomePage'
import PhonePage from './components/PhonePage'

export default {
  name: 'app',
  data () {
    return {
      f7params: {
        routes: [
          {
            path: '/',
            component: HomePage
          },
          {
            path: '/phone',
            component: PhonePage
          }
        ],
        name: 'Framework7',
        id: 'io.framework7.testapp',
        theme: 'auto'
      }
    }
  }
}
</script>
<style lang="scss">
@import "~framework7/css/framework7.min.css";
@import '~vue-phone-number-input/dist/vue-phone-number-input.css';
</style>
