<template>
    <div class="home has-navbar-fixed-top">
        <section class="hero is-light is-fullheight">
            <div class="hero-head">
                <div class="container is-fluid has-text-centered">
                    <img src="../assets/rahul.jpg" width="200" height="400" alt="Rahul Popuri">
                    <h1 class="title">
                        Rahul Popuri
                    </h1>
                    <h2 class="subtitle">
                        Java Developer
                    </h2>
                </div>
            </div>
            <div class="hero-body">
                <div class="container is-fluid has-text-centered">
                    <h2 class="title">
                        Skills
                    </h2>
                    <span class="tag is-info">Java</span>
                    <span class="tag is-info">Spring Boot</span>
                    <span class="tag is-info">SQL Server</span>
                    <span class="tag is-info">MySQL</span>
                    <span class="tag is-info">Google Cloud</span>
                    <span class="tag is-warning">Android</span>
                    <span class="tag is-warning">Tableau</span>
                    <span class="tag is-warning">Python</span>
                    <span class="tag is-warning">MongoDB</span>
                    <span class="tag is-warning">Redis</span>
                </div>
            </div>
        </section>
    </div>
</template>

<script>

export default {
  name: 'about',
  data: function () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='sass' scoped>
@import '../mq'

</style>
