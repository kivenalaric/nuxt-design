<template>
    <h2 class="h2_tag">{{ heading }}</h2>
</template>

  
<script>

export default {
    name: "H2",
    props: {
        heading: String,
    }
};
</script>
  
<style scoped>
.h2_tag {
    color: #000;
    font-size: 1.6rem;
    line-height: 1.2rem;
    text-align: left;
    font-weight: 700;
    align-self: flex-start;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    margin: 0;
}

@media (max-width: 600px) {
    .h2_tag {
        font-size: 1.2rem;
        text-align: center;
        align-self: center;
    }
}
</style>
  