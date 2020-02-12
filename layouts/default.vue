<template lang="pug">
div
  nav.uk-navbar-container.uk-margin(uk-navbar)
    .uk-navbar-left
      a.uk-navbar-item.uk-logo(href='#') 
      
        i.fas.fa-sun.fa-2x.uk-margin-small-right
        | Engenho Novo Opus 8
      ul.uk-navbar-nav
        li
          a(href='#')
            span.uk-icon.uk-margin-small-right(uk-icon='icon: waves')  Category Seven
      ul.uk-navbar-nav
        li
          a(href='#')
            span.uk-icon.uk-margin-small-right(uk-icon='icon: waves')  Category Twelve        
      .uk-navbar-item
      .uk-navbar-item
        form(action='javascript:void(0)')
          input.uk-input.uk-form-width-small(type='text' placeholder='Input')
          button.uk-button.uk-button-primary.uk-margin-small-left Data Input 

  nuxt      
</template>

<script>
import MyFooter from '~/components/Footer.vue'

export default {
  components: {
    MyFooter
  }
}
</script>

<style>
.container
{
  margin: 0;
  width: 100%;
  padding: 100px 0;
  text-align: center;
}

.button, .button:visited
{
  display: inline-block;
  color: black;
  letter-spacing: 1px;
  background-color: #fff;
  border: 2px solid #000;
  text-decoration: none;
  text-transform: uppercase;
  padding: 15px 45px;
}

.button:hover, .button:focus
{
  color: #fff;
  background-color: #000;
}

.title
{
  color: #000;
  font-weight: 300;
  font-size: 2.5em;
  margin: 0;
}
</style>
