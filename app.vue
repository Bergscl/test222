<template>
  <div>
    <el-button type="primary" @click="handleClick">打开弹窗</el-button>
    <eve-dialog-base title="标" v-if="visible" @close="visible = false">
      <div>弹1t</div>
    </eve-dialog-base>
  </div>
</template>
<script>
export default {
  data() {
    return {
      visible: false,
    };
  },
  methods: {
    handleClick() {
      this.visible = true;
    },
  },
};
</script>
