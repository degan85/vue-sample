<template lang="html">
  <b-card-group deck class="p-4">
      <b-card
      center
        v-for="(todoItem, index) in propsdata"
        :key="todoItem"
        img-src="./src/assets/images/1.jpg"
        img-alt="Card image"
        img-top>
        <p class="card-text">
          {{ todoItem }}
        </p>
      </b-card>
  </b-card-group>
</template>

<script>
export default {
  props: ['propsdata'],
}
</script>

<style lang="css" scoped>
.card {
  min-width: 300px;
}
</style>
