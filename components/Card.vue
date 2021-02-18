<template>
  <nuxt-link :to="slug">
    <article class="border p-4 rounded my-4">
      <h2 class="text-xl font-bold">{{ title }}</h2>
      <time class="text-right text-sm text-gray-700">{{ date }}</time>
      <div class="tags">
        <Tag>{{ category }}</Tag>
      </div>
    </article>
  </nuxt-link>
</template>

<script>
// eslint-disable-next-line no-unused-vars
import Tag from '~/components/Tag'

export default {
  props: {
    // eslint-disable-next-line vue/require-default-prop
    title: String,
    // eslint-disable-next-line vue/require-default-prop
    date: String,
    // eslint-disable-next-line vue/require-default-prop
    category: String,
    // eslint-disable-next-line vue/require-default-prop
    slug: String,
  },
}
</script>

<style></style>
