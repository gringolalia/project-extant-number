<template lang="pug">
section.container
  img.logo(src='~assets/img/hammer-sickle.svg' alt='Spectre Haunts' width="175px;")
  h1.uk-margin-small  None More Excellent Twice
  h2.uk-margin-small Lost In Uffish Thought 
  button.uk-button.uk-button-secondary.uk-margin-small Full Court Press Me
</template>

<script>
import axios from '~/plugins/axios'

export default {
  async asyncData () {
    let { data } = await axios.get('/api/users')
    return { users: data }
  },
  head () {
    return {
      title: 'Users'
    }
  }
}
</script>

<style scoped>
.title
{
  margin: 30px 0;
}
.users
{
  list-style: none;
  margin: 0;
  padding: 0;
}
.user
{
  margin: 10px 0;
}
</style>
