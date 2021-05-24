<template>
  <div class="flex flex-col justify-center items-center w-full min-h-screen">
    <a-heading
      tag="h1"
      :variant="['first-level', 'font-secondary']"
      class="mb-4"
    >
      Alpaca UI
    </a-heading>
    <a-heading
      tag="h2"
      :variant="['second-level']"
      class="mb-4"
    >
      Nuxt Playground
    </a-heading>
    <a-price
      regular-price="$100,00"
      class="mb-4"
    />
    <a-price
      regular-price="$36,00"
      special-price="$19,90"
      aria-label-special-price="Price reduced from:"
      aria-label-old-price="On sale at:"
    />

    <a-heading
      tag="h3"
      :variant="['first-level', 'font-secondary']"
      class="mb-4"
    >
      App Breadcrubms component - build from Alpaca-ui parts
    </a-heading>
    <app-breadcrumbs :breadcrumbs="breadcrumbs" />

    <a-heading
      tag="h3"
      :variant="['first-level', 'font-secondary']"
      class="mb-4"
    >
      ABreadcrubms component - import the whole component from Alpaca-ui
    </a-heading>
    <a-breadcrumbs :breadcrumbs="breadcrumbs" />
  </div>
</template>

<script>
import { Heading, Price, Breadcrumbs } from '@snowdog/alpaca-ui'
import AppBreadcrumbs from '~/components/AppBreadcrumbs'

export default {
  components: {
    AHeading: Heading,
    APrice: Price,
    ABreadcrumbs: Breadcrumbs,
    AppBreadcrumbs
  },
  data () {
    return {
      breadcrumbs: [
        {
            'text': 'Home',
            'href': '#'
          },
          {
            'text': 'category2',
            'href': '#'
          },
          {
            'text': 'category3',
            'href': '#'
          },
          {
            'text': 'category4',
            'href': '#'
          }
      ]
    }
  }
}
</script>
