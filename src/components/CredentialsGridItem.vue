<template>
  <div class="credential-item">
    <span class="text-lg">{{item.name}}</span>
    <span>URL: {{item.url}}</span>
    <span>Userame: {{item.username}}</span>
    <router-link v-bind:to="`/credentials/${item.id}`">Details</router-link>
  </div>
</template>

<script>
export default {
  name: "CredentialsGridItem",
  props: [
    "item"
  ]
}
</script>