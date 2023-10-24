<template>
  <button @click="onClick()" class="button" :color="buttonColor" type="button">
    {{ text }}
    <span class="span">{{ time }}</span>
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    color: String,
    width: String,
    buttonColor: String,
    time: String
  },
  methods: {
    onClick() {
      this.$emit('btn-click');
    }
  }
}
</script>

<style scoped>
.button {
  background: #000;
  color: #fff;
  border: none;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0.6rem 1.2rem;
  width: 90vw;
  margin: 0 10px;
  max-width: 400px;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  border-radius: 1.8rem;
  text-align: center;
  cursor: pointer;
  text-decoration: none;
  font-size: 20px;
}

.span {
  font-size: 14px;
  text-align: center;
  font-weight: 100;
}

@media (max-width: 600px) {
  .button {
    padding: 5px;
    font-size: 16px;
    margin: 0 0.5rem;
  }
}
</style>
