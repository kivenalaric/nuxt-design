<template>
  <p class="p_footer">
    {{ text }}
    <span class="span_f">
      {{ span }}
    </span>
  </p>
</template>

<script>
export default {
  name: "Pfooter",
  props: {
    text: String,
    span: String
  }
}
</script>

<style>
.p_footer {
  display: flex;
  align-items: center;
  gap: 8px;
  color: #000;
  font-size: 20px;
  font-weight: 500;
  padding: 0 0 5px;
  opacity: 1;
  letter-spacing: 0;
  margin-bottom: 0;
  margin-top: 0.5rem;
  align-self: flex-start;
  text-align: left;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

.span_f {
  color: #d9bb6a;
  font-weight: 600;
  cursor: pointer;
}
</style>
