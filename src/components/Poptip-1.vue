<demo>
基础用法
</demo>
<template>
<Poptip trigger='click'>
  <template v-slot:content>
    <div>气泡提示内容</div>
  </template>
  <Button>click 激活</Button>
</Poptip>

<Poptip trigger='hover'>
  <template v-slot:content>
    <div>气泡提示内容</div>
  </template>
  <Button>hover 激活</Button>
</Poptip>
</template>

<script lang="ts">
import Poptip from "../lib/Poptip.vue";
import Button from "../lib/Button.vue";
export default {
  components: {
    Poptip,
    Button,
  },
};
</script>
