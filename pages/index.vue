<template>
  <section>
    <div>
      <logo/>
      <h1 class="subtitle">Nuxt + UIKit</h1>
      <h1 class="uk-heading-line uk-text-center"><span>Simple example of integration with UIKit</span></h1>
        
      <div class="links" uk-margin>
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="uk-button uk-button-primary">Nuxt Docs</a>
        <a
          href="https://getuikit.com/docs/introduction"
          target="_blank"
          class="uk-button uk-button-secondary">UIKit Docs</a>
        <nuxt-link
        class="uk-button uk-button-default"
        title="UIkit tooltip" uk-tooltip
        to="/about"
        >This is UIKit button, CLICK ME!</nuxt-link>
            
      </div>
 
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'
import IconLink from '~/components/IconLink.vue'

export default {
  components: {
    Logo,
    IconLink
  }
}
</script>

<style scoped>
.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 400; 
  font-size: 100px;
  color: #526488;
  letter-spacing: 1px;
  font-size: 6em;
}

.subtitle {
  font-weight: 300;
  font-size: 3em;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
