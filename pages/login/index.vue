<template>
  <div>
    <div class="login" @click="login">Login and  To '/user/info'</div>
  </div>
</template>

<script setup lang="ts">
definePageMeta({
    layout: false
})

const login = () => {
  useRouter().push('/user/info')
}
</script>

<style scoped>
.login{
  height: 48px;
  line-height: 48px;
  padding: 0 12px;
  border-radius: 4px;
  background-color: #00DC82;
  display: inline-block;
  font-family: monospace;
  font-size: 18px;
  cursor: pointer;
}
</style>