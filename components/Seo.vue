<template>
  <div>
    <Head>
      <Title>{{ title }}</Title>
    </Head>
  </div>
</template>

<script setup>
const props = defineProps({
  title: String,
});

console.log(props);
</script>

<style lang="scss" scoped>
</style>