<template>
  <div class="sec1_cards" v-for="item in mapArr" :key="item.id">
    <Icon :name="item.icon" />
    <Ptag :text="item.text" class="cardp" />
    <Ptag :text="item.desc" class="cardps" />
  </div>
</template>

<script>
import Ptag from '../atoms/Ptag.vue';
import Icon from '../atoms/Icons.vue';

export default {
  name: "Card1",
  components: {
    Ptag,
    Icon
  },
  props: {
    mapArr: Array,
  },
  data() {
    return {
      mapArr: this.mapArr
    }
  }
}

</script>

<style scoped>
.sec1_cards {
  padding: 1.2rem 0.5rem;
  width: 90vw;
  max-width: 262px;
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