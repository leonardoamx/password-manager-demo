<template>
  <div class="credentials mx-8 my-8">
    <h1 class="text-bold text-lg">Store your account credentials in a single place</h1>
    <p>Entries: {{credentialsTotal}}</p>
    <CredentialsGrid
      :items="credentials"
    />
  </div>
</template>

<script>
import {credentials} from "@/assets/initialData.js"
import CredentialsGrid from "@/components/CredentialsGrid.vue"

export default {
  name: 'CredentialsView',
  components: {
    CredentialsGrid
  },
  data() {
    return {
      credentials
    }
  },
  computed: {
    credentialsTotal() {
      return credentials.length;
    }
  }
}
</script>
