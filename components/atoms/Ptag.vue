<template>
  <p class="p_tag">{{ text }}</p>
</template>

<script>

export default {
  name: "Ptag",
  props: {
    text: String,
  },
};
</script>

<style scoped>
.p_tag {
  color: #000;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  text-align: center;
}
</style>
