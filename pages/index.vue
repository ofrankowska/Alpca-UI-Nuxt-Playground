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
  </div>
</template>

<script>
import { Heading, Price } from '@snowdog/alpaca-ui'
export default {
  components: {
    AHeading: Heading,
    APrice: Price
  }
}
</script>
