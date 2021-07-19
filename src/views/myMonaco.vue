<template>
  <div id="monaco" class="editor">
  </div>
</template>
<script>
import * as monaco from "monaco-editor";
export default {
  mounted() {
    const model=monaco.editor.createModel("console.log('aiqiyi')","javascript"); 
    monaco.editor.create(document.getElementById("monaco"), {
      model:model,
      foldingStrategy: 'indentation', // 代码可折叠
      automaticLayout: true, // 自适应布局
      BuiltinTheme:'vs-dark'
    });
  },
};
</script>
<style lang="scss" scoped>
    .editor {
        height: 100vh;
    }
</style>
