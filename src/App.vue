<template>
  <div id="app">
    <nav class="navbar ">
      <div class="navbar-brand">
        <div class="navbar-burger burger" onclick="document.querySelector('.navbar-menu').classList.toggle('is-active'); document.querySelector('.navbar-burger').classList.toggle('is-active');">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
      <div class="navbar-menu">
        <div class="navbar-start">
          <div class="navbar-item is-hoverable">
             <router-link to="/" class="navbar-item is-active">Home</router-link>
          </div>
          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link" >
              Projects
            </a>
            <div class="navbar-dropdown ">
              <a class="navbar-item " href="https://play.google.com/store/apps/details?id=ca.bubblewrapstudios.mailinglist" target="_blank">
                Mailing List
              </a>
              <a class="navbar-item " href="http://twine.bubblewrapstudios.ca" target="_blank">
                Twine
              </a>
              <a class="navbar-item " href="https://github.com/rahulpopuri/tvmaze-java" target="_blank">
                TvMaze API
              </a>
              <a class="navbar-item " href="https://github.com/rahulpopuri/plants" target="_blank">
                Plants
              </a>
              <a class="navbar-item " href="http://twine.bubblewrapstudios.ca" target="_blank">
                URL Shortener
              </a>
            </div>
          </div>
          <div class="navbar-item">
             <a href="https://500px.com/rahulpopuri" target="_blank">Photography</a>
          </div>
        </div>
        <div class="navbar-end">
          <div class="navbar-item">
            <div class="field is-grouped">
              <p class="control">
                <a href="https://drive.google.com/open?id=1RXFHtcyVrSRpmWZc4NIdqGLvkunBQZt0" target="_blank">
                    Resume
                </a>
              </p>
              <p class="control">
                <a class="icon" href="https://github.com/rahulpopuri">
                    <i class="fa fa-github" aria-hidden="true"></i>
                </a>
              </p>
              <p class="control">
                <a class="icon" href="https://www.linkedin.com/in/rahulpopuri/">
                    <i class="fa fa-linkedin" aria-hidden="true"></i>
                </a>
              </p>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang='sass' scoped>
@import 'mq'

</style>
