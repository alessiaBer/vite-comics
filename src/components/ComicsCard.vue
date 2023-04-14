<script>
export default {
    name: 'ComicsCard',
    props: {
      title: String,
      img: String,
    }
};
</script>

<template>
  <div class="col">
    <div class="my_card">
      <img :src="img" :alt="title">
      <h5>{{ title.toUpperCase() }}</h5>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
