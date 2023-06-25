<template>
  <main>
    <div class="card flex justify-content-center flex-wrap gap-3">
      <Button label="Primary" />
      <Button label="Secondary" severity="secondary" />
      <Button label="Success" severity="success" />
      <Button label="Info" severity="info" />
      <Button label="Warning" severity="warning" />
      <Button label="Help" severity="help" />
      <Button label="Danger" severity="danger" />
    </div>
    <div class="card flex justify-content-center flex-wrap gap-3">
      <Button label="Primary" text raised />
      <Button label="Secondary" severity="secondary" text raised />
      <Button label="Success" severity="success" text raised />
      <Button label="Info" severity="info" text raised />
      <Button label="Warning" severity="warning" text raised />
      <Button label="Help" severity="help" text raised />
      <Button label="Danger" severity="danger" text raised />
      <Button label="Plain" plain text raised />
    </div>
    <div class="card flex justify-content-center flex-wrap gap-3">
      <Button type="button" label="Emails" badge="8" />
      <Button
        type="button"
        label="Messages"
        icon="pi pi-users"
        badge="8"
        badgeClass="p-badge-danger"
        outlined
      />
    </div>
    <div class="card flex justify-content-center">
      <Button type="button" label="Search" icon="pi pi-search" :loading="loading" @click="load" />
    </div>
  </main>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import Button from 'primevue/button'

const loading = ref(false)

const load = () => {
  loading.value = true
  setTimeout(() => {
    loading.value = false
  }, 2000)
}
</script>
