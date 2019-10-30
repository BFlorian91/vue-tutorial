<template>
  <div>
    <img :src="url.src" :alt="person.firstname">
    <h1>Hello from {{ from }},</h1>
    <h3>by {{ name }} {{ surname }}</h3>
  </div>
</template>

<script>
export default {
  data () {
    return {
      person: {
        firstname: 'Homer',
        lastname: 'Simpson'
      },
      url: {
        src: 'http://www.slate.fr/sites/default/files/styles/1060x523/public/homer-simpson_0.jpg'
      },
      from: 'Springfield'
    }
  },
  props: [
    'name',
    'surname'
  ]
}
</script>

<style>

</style>