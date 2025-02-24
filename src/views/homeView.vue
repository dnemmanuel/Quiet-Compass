<template>
  <div>
    <lines />
  </div>
</template>

<script>
import lineData from "../dataSheets/lineData.json";
import lines from "../components/lineItem.component.vue";
export default {
  name: "home",

  components: {
    lines,
  },

  data() {
    return {};
  },
};
</script>
