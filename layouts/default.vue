<template>
  <div>
    <div class="header">
      Default Layout
    </div>
    <div>
      <slot />
    </div>
  </div>
</template>

<script setup lang="ts">
onMounted(() => {
  console.log(useRouter().currentRoute.value.path)
  console.log(useRoute().path)
})
</script>

<style scoped>
.header{
  height: 48px;
  border-bottom: 1px solid #e3e3e3;
  font-size: 24px;
  color: #017947;
}
</style>