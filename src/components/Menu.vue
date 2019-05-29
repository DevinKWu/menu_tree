<template>
  <ul class="menu">
    <MenuItem v-for="(menu,index) in menuList" :item="menu" :key="index"/>
  </ul>
</template>

<script>
import MenuItem from "./MenuItem";
export default {
  components: {
    MenuItem
  },
  props: {
    menuList: {
      type: Object,
      required: true
    }
  }
};
</script>
