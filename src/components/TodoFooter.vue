<template lang="html">
    <div class="clearAllContainer">
      <span class="clearAllBtn" @click="clearTodo">Clear All</span>
    </div>
</template>

<script>
export default {
  methods: {
    clearTodo() {
      // 클릭하면 removeAll 이벤트를 발생시킴
      // 상위 컴포넌트 App.vue로 전달
      // 상위 컴포넌트에서 removeAll을 받아 clearAll()메서드를 실행
      this.$emit('removeAll');
    }
  }
}
</script>

<style lang="css">
.clearAllContainer {
  width: 8.5rem;
  height: 50px;
  line-height: 50px;
  background-color: white;
  border-radius: 5px;
  margin: 0 auto;
}

.clearAllBtn {
  color: #e20303;
  display: black;
}
</style>
rf85m91627x
wd21j9830kv
328
