<template>
  <md-editor v-model="text" :theme="theme"></md-editor>
  
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";
import MdEditor from "md-editor-v3";
import "md-editor-v3/lib/style.css";

export default defineComponent({
  name: "MdEditor",
  components: {
    MdEditor,
  },
  setup() {
    const text = ref("");
    const theme = ref("light");

    return {
      text,
      theme,
    };
  },
});
</script>
