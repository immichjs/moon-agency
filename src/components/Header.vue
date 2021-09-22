<template>
  <header class="header">
    <div class="header__container">
      <img class="header__container-logo" src="../assets/img/moon-logo.png">
      <box-icon class="menu-burger" name='menu-alt-right'></box-icon>
      <nav class="nav">
        <ul class="nav__container">
          <li class="nav__container-item">Home</li>
          <li class="nav__container-item">Service</li>
          <li class="nav__container-item">Portifolio</li>
          <li class="nav__container-item">Blog</li>
          <li class="nav__container-item">Feeds</li>
        </ul>
      </nav>
    </div>
    <button class="header__contact">Contact Us</button>
  </header>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
})
</script>

<style lang="sass" scoped>
@import '../assets/sass/base/variables'

.header
  align-items: flex-end
  display: flex
  height: 5rem
  justify-content: space-between
  margin: 0 12rem

  &__container
    display: flex
    gap: 4rem

    &-logo
      width: 4rem
      height: 4rem

    .menu-burger
      display: none

    .nav
      &__container
        align-items: center
        display: flex
        gap: .5rem
        height: 100%

        &-item
          align-items: center
          border-bottom: 1px solid transparent
          border-radius: .15rem
          color: $gray-color-50
          cursor: pointer
          display: flex
          font-size: .9rem
          font-weight: 600
          letter-spacing: .075rem
          padding: 1rem
          transition: .3s
        
          &:hover
            background-color: darken($purple-color-bg, 1%)
            border-color: #f5f5f544
            transform: translateY(-.25rem)

  &__contact
    padding: .75rem 2rem
    background: transparent
    border: 2px solid $gray-color-50
    border-radius: 50px
    color: $gray-color-50
    font-size: .9rem
    font-weight: 600
    transition: .3s
    cursor: pointer
    box-shadow: 0 0 10px rgba(0, 0, 0, .075)

    &:hover
      background-color: $gray-color-50
      color: $gray-color-700

</style>
