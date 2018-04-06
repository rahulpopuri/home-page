<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}

function closeDropdownsIfAnyClick (ev) {
  'use strict'

  var tgt = ev.target || ev.srcElement

  // close all (but allow open just clicked)
  document.querySelectorAll('.has-dropdown input[type="checkbox"]').forEach(
    function (chb) {
      if (chb.id !== tgt.id && chb.id !== tgt.getAttribute('for')) { chb.checked = false }
    }
  )

  return true
}

document.querySelector('body').addEventListener('click', closeDropdownsIfAnyClick)
</script>

<style lang='sass' scoped>
@import 'mq'
.navbar-item a
    font-weight:bold

a.navbar-item,
.navbar-link
    color: black
    padding: 0.5rem 1.75rem
    font-weight: normal

a.navbar-item,
a.navbar-link
    &:hover,
    &.is-active
        background-color: $navbar-item-hover-background-color
        color: $navbar-item-hover-color

.icon
  color: black
</style>
