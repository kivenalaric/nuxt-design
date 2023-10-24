<template>
  <div class="bot_main">
    <H2 :heading="myTitle" />
    <div class="bottom_sec">
      <Card3 />
    </div>
  </div>
</template>

<script>

import H2 from "@/components/atoms/H2.vue";
import Card3 from '@/components/molecules/Sec3card.vue';

export default {
  name: "BottomSec",
  components: {
    H2,
    Card3
  },
  data() {
    return {
      myTitle: "Tools"
    }
  }
}

</script>

<style>
.bot_main {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  gap: 0.5rem;
}

.bottom_sec {
  display: grid;
  grid-template-columns: auto auto auto;
  align-items: center;
  justify-content: space-between;
  margin: auto;
  width: 97vw;
  max-width: 1150px;
  gap: 1rem;
}

@media (max-width: 600px) {
  .bottom_sec {
    display: flex;
    flex-direction: column;
  }
}
</style>

