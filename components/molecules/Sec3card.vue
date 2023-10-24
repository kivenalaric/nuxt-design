<template>
  <div class="sec3_cards" v-for="item in sec3Arr" :key="item.id">
    <Icon :name="item.icon" />
    <Ptag :text="item.text" class="cardp" />
    <Ptag :text="item.desc" class="cardps" />
  </div>
</template>


<script>
import Icon from '@/components/atoms/Icons.vue';
import Ptag from '@/components/atoms/Ptag.vue';
import { sec3Arr } from "../../arrays/array.js";

export default {
  name: "Card3",
  components: {
    Ptag,
    Icon,
  },
  data() {
    return {
      sec3Arr
    }
  }
}
</script>

<style>
.sec3_cards {
  padding: 1.2rem 0.5rem;
  width: 90vw;
  max-width: 338px;
  display: flex;
  flex-direction: column;
  margin: auto;
  align-items: center;
  justify-content: center;
  background: #d9bb6aff;
  color: #000;
  border-radius: 0.8rem;
  border: 3px solid #000;
}

.cardp {
  font-weight: 700;
  font-size: 20px;
  margin-bottom: 0;
}

.cardps {
  font-size: 14px;
  margin: 0 auto;
  line-height: 1rem;
  font-weight: 0;
}
</style>