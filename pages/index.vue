<template>
  <section class="container">
    <div class="wrapper">
      <LogoName/>
    </div>
  </section>
</template>

<script>
import Skills from '~/components/Skills.vue'
import LogoName from '~/components/LogoName.vue'

export default {
  components: {
    Skills,
    LogoName
  },
  
  computed: {
    skills()
    {
      return [
        {weight: 2, label: 'Laravel'},
        {weight: 2, label: 'VueJS'},
        {weight: 0, label: 'JavaScript'},
        {weight: 2, label: 'PHP'},
        {weight: 1, label: 'Tailwind CSS'},
        {weight: 1, label: 'Bulma'},
        {weight: 0, label: 'Bootsrap'},
        {weight: 2, label: 'MySQL'},
        {weight: 0, label: 'Docker'},
        {weight: 1, label: 'Linux'},
        {weight: 2, label: 'Git'},
        {weight: 1, label: 'Webpack'},
        {weight: 0, label: 'Sass'},
        {weight: 0, label: 'NativeScript Vue'},
        {weight: 1, label: 'Python'},
        {weight: 1, label: 'Django'},
        {weight: 0, label: 'React'},
        {weight: 0, label: 'React Native'},
        {weight: 1, label: 'Yarn'},
        {weight: 1, label: 'NPM'},
        {weight: 0, label: 'Expression Engine'},
        {weight: 0, label: 'Wordpress'},
        {weight: 0, label: 'NodeJS'},
      ];
    }
  }
}
</script>

<style lang="scss">

$master-color: #35495e;

.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}

.title {
  width: 580px;
  padding: 1rem;
  font-size: 3rem;
  font-weight: 300;
  color: $master-color;
  @apply flex items-center justify-around;
  border: 1px solid $master-color;
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
}

.skills {
  font-weight: 300;
  font-size: 1rem;
  color: #526488;
  word-spacing: 5px;
  padding-left: 10rem;
  padding-right: 10rem;
  padding-bottom: 15px;
  @apply flex items-center flex-wrap justify-center;
}

.skills .skill {
  margin-right: .5rem;
}

.links {
  padding-top: 15px;
}
</style>
