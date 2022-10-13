<template>
  <div class="grid-wrap">
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