<template>
  <div class="about">
    <h1>This is an about page</h1>
    <div class="demo-split">
      <Split v-model="split1">
        <div slot="left" class="demo-split-pane">Left Pane</div>
        <div slot="right" class="demo-split-pane">Right Pane</div>
      </Split>
    </div>
  </div>
</template>
<script>
export default {
  name: "About",
  data() {
    return {
      split1: "300px"
    };
  }
};
</script>
<style>
.demo-split {
  height: 200px;
  border: 1px solid #dcdee2;
}
.demo-split-pane {
  padding: 10px;
}
</style>