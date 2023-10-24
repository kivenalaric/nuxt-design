<template>
  <div class="mid_main">
    <H2 :heading="myTitle" />
    <div class="mid_sec">
      <Card2 />
    </div>
    <Pfooter :text="p1" :span="span" style="font-size: 1.5rem; width: 80vw; max-width: 900px" />
  </div>
</template>

<script>
import Pfooter from '@/components/atoms/Pfooter.vue';
import H2 from "@/components/atoms/H2.vue";
import Card2 from '@/components/molecules/Sec2card.vue';


export default {
  name: "MiddleSec",
  components: {
    H2,
    Card2,
    Pfooter
  },
  data() {
    return {
      myTitle: "Get Help",
      p1: "Confused by all the Tech Talk?",
      span: "Visit our Tech Glossary Here!!!"
    }
  }
}

</script>

<style>
.mid_main {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  gap: 0.5rem;
}

.mid_sec {
  display: flex;
  flex-direction: row;
  align-items: center;
  width: 97vw;
  margin: auto;
  justify-content: space-between;
  gap: 0.8rem;
  max-width: 1150px;
}

@media (max-width: 600px) {
  .mid_sec {
    display: grid;
    grid-template-columns: auto auto;
  }
}
</style>

