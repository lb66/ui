<template>
<div class="ui-buttonGroup">
  <slot />
</div>
</template>

<script lang="ts">
export default {};
</script>

<style lang="scss">
.ui-buttonGroup {
  display: inline-flex;
  vertical-align: middle;

  &+& {
    margin-left: 10px;
  }

  >.ui-button {
    border-radius: 0;
    margin-left: -1px;

    &:first-child {
      border-top-left-radius: 4px;
      border-bottom-left-radius: 4px;
    }

    &:last-child {
      border-top-right-radius: 4px;
      border-bottom-right-radius: 4px;
    }

    &:hover {
      position: relative;
      z-index: 1;
    }
  }
}
</style>
