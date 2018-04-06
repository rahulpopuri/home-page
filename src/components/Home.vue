<template>
    <div class="home">
        <section class="hero is-light is-fullheight">
            <div class="hero-body">
                <div class="container is-fluid has-text-centered">
                    <section class="section">
                        <div class="columns is-desktop is-vcentered">
                            <div class="column has-text-right-desktop">
                                <img src="../assets/rahul.jpg" width="200" height="200" alt="Rahul Popuri">
                            </div>
                            <div class="column has-text-left-desktop">
                                <section class="section">
                                    <h1 class="title">
                                        Rahul Popuri
                                    </h1>
                                    <h1 class="subtitle is-size-6">
                                        Backend Developer
                                    </h1>
                                    <a class="has-text-black has-text-weight-semi-bold" href="https://drive.google.com/open?id=1RXFHtcyVrSRpmWZc4NIdqGLvkunBQZt0" target="_blank">
                                        Resume
                                    </a>
                                    <a class="icon" href="https://github.com/rahulpopuri">
                                        <i class="fa fa-github" aria-hidden="true"></i>
                                    </a>
                                    <a class="icon" href="https://www.linkedin.com/in/rahulpopuri/">
                                        <i class="fa fa-linkedin" aria-hidden="true"></i>
                                    </a>
                                    <a class="icon" href="https://500px.com/rahulpopuri">
                                        <i class="fa fa-500px" aria-hidden="true"></i>
                                    </a>
                                </section>
                                <section class="section">
                                    <div class="dropdown">
                                        <div class="dropdown-trigger">
                                            <button class="button" aria-haspopup="true" aria-controls="dropdown-menu2">
                                            <span>Projects</span>
                                            <span class="icon is-small">
                                                <i class="fa fa-angle-down" aria-hidden="true"></i>
                                            </span>
                                            </button>
                                        </div>
                                        <div class="dropdown-menu" id="dropdown-menu2" role="menu">
                                            <div class="dropdown-content has-text-left">
                                                <div class="dropdown-item">
                                                    <a href="https://play.google.com/store/apps/details?id=ca.bubblewrapstudios.mailinglist" target="_blank">
                                                        Mailing List
                                                    </a>
                                                </div>
                                                <hr class="dropdown-divider">
                                                <a class="dropdown-item " href="http://twine.bubblewrapstudios.ca" target="_blank">
                                                    Twine
                                                </a>
                                                <hr class="dropdown-divider">
                                                <a class="dropdown-item " href="https://github.com/rahulpopuri/tvmaze-java" target="_blank">
                                                    TvMaze API
                                                </a>
                                                <hr class="dropdown-divider">
                                                <a class="dropdown-item " href="https://github.com/rahulpopuri/plants" target="_blank">
                                                    Plants
                                                </a>
                                                <hr class="dropdown-divider">
                                                <a class="dropdown-item " href="https://github.com/rahulpopuri/url-shortener" target="_blank">
                                                    URL Shortener
                                                </a>
                                            </div>
                                        </div>
                                    </div>
                                </section>
                            </div>
                        </div>
                    </section>
                    <section class="section">
                        <h2 class="title">
                            Skills
                        </h2>
                        <span class="tag is-info ">Java</span>
                        <span class="tag is-info">Spring Boot</span>
                        <span class="tag is-info">SQL Server</span>
                        <span class="tag is-info">MySQL</span>
                        <span class="tag is-info">Google Cloud</span>
                        <span class="tag is-warning">Android</span>
                        <span class="tag is-warning">Tableau</span>
                        <span class="tag is-warning">Python</span>
                        <span class="tag is-warning">MongoDB</span>
                        <span class="tag is-warning">Redis</span>
                    </section>
                </div>
            </div>
        </section>
    </div>
</template>

<script>

export default {
  name: 'about'
}
document.addEventListener('DOMContentLoaded', function () {
  var $dropdowns = getAll('.dropdown:not(.is-hoverable)')

  if ($dropdowns.length > 0) {
    $dropdowns.forEach(function ($el) {
      $el.addEventListener('click', function (event) {
        event.stopPropagation()
        $el.classList.toggle('is-active')
      })
    })

    document.addEventListener('click', function (event) {
      closeDropdowns()
    })
  }

  function closeDropdowns () {
    $dropdowns.forEach(function ($el) {
      $el.classList.remove('is-active')
    })
  }

  // Close dropdowns if ESC pressed
  document.addEventListener('keydown', function (event) {
    var e = event || window.event
    if (e.keyCode === 27) {
      closeDropdowns()
    }
  })

  // Functions

  function getAll (selector) {
    return Array.prototype.slice.call(document.querySelectorAll(selector), 0)
  }
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='sass' scoped>
@import '../mq'

</style>
