<template>
  <div>
    <ChildComp />
  </div>
</template>

<script>
export default {
  components: {
    ChildComp: {
      methods: {
        heavy() {
          /* 耗时任务 */
        },
      },
      render(h) {
        return h("div", this.heavy());
      },
    },
  },
};
</script>
