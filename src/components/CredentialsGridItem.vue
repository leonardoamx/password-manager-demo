<template>
  <div class="credential-item rounded-lg bg-white p-4 shadow-xl shadow-black/5 hover:bg-slate-50 ring-2 ring-indigo-600">
    <div class="flex justify-between">
      <div class="font-bold text-slate-900">{{item.name}}</div>
    </div>
    <div class="mt-1 text-slate-700">
      <span class="font-bold">URL: </span>
      <span>{{item.url}}</span>
    </div>
    <div class="mt-1 text-slate-700">
      <span class="font-bold">Username: </span>
      <span>{{item.username}}</span>
    </div>
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