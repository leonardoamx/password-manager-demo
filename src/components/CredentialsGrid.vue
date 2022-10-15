<template>
  <div class="grid-wrap grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-4">
    <CredentialsGridItem
      v-for="item in items"
      :key="item.id"
      :item="item"
    />
  </div>
</template>

<script>
import CredentialsGridItem from "@/components/CredentialsGridItem.vue"

export default {
  name: "CredentialsGrid",
  props: [
    "items"
  ],
  components: {
    CredentialsGridItem
  }
}
</script>
