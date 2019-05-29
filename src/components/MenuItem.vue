<template>
  <li class="item">
    <span v-if="hasChild" @click="toggleOpen">{{opened ? '-' : '+'}}</span>
    <a href="javascript:;">{{ item.label }}</a>
    <Menu :menuList="item.children" v-show="hasChild && opened"></Menu>
    <!-- <ul v-show="hasChild && opened">
      <MenuItem v-for="(child,index) in item.children" :key="index" :item="child"/>
    </ul>-->
  </li>
</template>

<script>
import Menu from "./Menu";
export default {
  name: "MenuItem",
  components: {
    Menu
  },
  props: {
    item: {
      type: Object,
      required: true
    }
  },
  data() {
    return {
      opened: false
    };
  },
  computed: {
    hasChild() {
      return this.item.children && this.item.children.length ? true : false;
    }
  },
  methods: {
    toggleOpen() {
      if (this.hasChild) {
        this.opened = !this.opened;
      }
    }
  }
};
</script>
