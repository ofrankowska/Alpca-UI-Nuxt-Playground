<template src="@molecules/breadcrumbs/Breadcrumbs.html" />

<script>
import ABreadcrumbs from '@molecules/breadcrumbs/Breadcrumbs.js'
import ALink from '@atoms/link/Link.vue'

export default {
  name: 'AppBreadcrumbs',
  mixins: [ABreadcrumbs],
  components: {
    ALink
  }
}
</script>
