<template>
  <div>
    <line />
  </div>
</template>

<script>
import lineData from "../dataSheets/lineData.json";
import line from "../components/lineItem.component.vue";
export default {
  name: "home",

  components: {
    line,
  },

  data() {
    return {};
  },
};
</script>
