<template>
  <div uk-margin >
  <nuxt-link to="/" class="uk-button uk-button-primary">Indietro</nuxt-link>
      <h1 class="subtitle">An example of UIkit Transition</h1>

<div class="uk-child-width-1-2 uk-child-width-1-3@s uk-grid uk-grid-match uk-grid-small" uk-grid>
    <div class="uk-text-center">
        <div class="uk-inline-clip uk-transition-toggle" tabindex="0">
            <img src="https://uploads.codesandbox.io/uploads/user/4f8528cb-ded4-4626-bbd0-971ae3c98c8d/G426-dark.jpg" alt="">
            <div class="uk-transition-fade uk-position-cover uk-position-small uk-overlay uk-overlay-default uk-flex uk-flex-center uk-flex-middle">
                <p class="uk-h4 uk-margin-remove">Fade</p>
            </div>
        </div>
        <p class="uk-margin-small-top">Fade</p>
    </div>
    <div class="uk-text-center">
        <div class="uk-inline-clip uk-transition-toggle" tabindex="0">
            <img src="https://uploads.codesandbox.io/uploads/user/4f8528cb-ded4-4626-bbd0-971ae3c98c8d/G426-dark.jpg" alt="">
            <div class="uk-transition-slide-bottom uk-position-bottom uk-overlay uk-overlay-default">
                <p class="uk-h4 uk-margin-remove">Bottom</p>
            </div>
        </div>
        <p class="uk-margin-small-top">Bottom</p>
    </div>
    <div class="uk-text-center">
        <div class="uk-inline-clip uk-transition-toggle uk-light" tabindex="0">
            <img src="https://uploads.codesandbox.io/uploads/user/4f8528cb-ded4-4626-bbd0-971ae3c98c8d/G426-dark.jpg" alt="">
            <div class="uk-position-center">
                <span class="uk-transition-fade" uk-icon="icon: plus; ratio: 2"></span>
            </div>
        </div>
        <p class="uk-margin-small-top">Icon</p>
    </div>
    <div class="uk-text-center">
        <div class="uk-inline-clip uk-transition-toggle" tabindex="0">
            <img src="https://uploads.codesandbox.io/uploads/user/4f8528cb-ded4-4626-bbd0-971ae3c98c8d/G426-dark.jpg" alt="">
            <img class="uk-transition-scale-up uk-position-cover" src="https://uploads.codesandbox.io/uploads/user/4f8528cb-ded4-4626-bbd0-971ae3c98c8d/LjIp-light.jpg" alt="">
        </div>
        <p class="uk-margin-small-top">2 Images</p>
    </div>
    <div class="uk-text-center">
        <div class="uk-inline-clip uk-transition-toggle" tabindex="0">
            <img class="uk-transition-scale-up uk-transition-opaque" src="https://uploads.codesandbox.io/uploads/user/4f8528cb-ded4-4626-bbd0-971ae3c98c8d/G426-dark.jpg" alt="">
        </div>
        <p class="uk-margin-small-top">Scale Up Image</p>
    </div>
    <div class="uk-text-center">
        <div class="uk-inline-clip uk-transition-toggle uk-light" tabindex="0">
            <img src="https://uploads.codesandbox.io/uploads/user/4f8528cb-ded4-4626-bbd0-971ae3c98c8d/G426-dark.jpg" alt="">
            <div class="uk-position-center">
                <div class="uk-transition-slide-top-small"><h4 class="uk-margin-remove">Headline</h4></div>
                <div class="uk-transition-slide-bottom-small"><h4 class="uk-margin-remove">Subheadline</h4></div>
            </div>
        </div>
        <p class="uk-margin-small-top">Small Top + Bottom</p>
    </div>
</div>
  </div>
</template>

<script>
export default {
  asyncData() {
    return {
      name: (process.server ? 'server' : 'client')
    }
  }
}
</script>

<style scoped>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
h1 {
  font-weight: 400;
}
.name {
  color: #3b8070;
}
p {
  margin-top: 20px;
}
</style>