<template>
    <div class="top_main">
        <H2 :heading="myTitle" />
        <div class="top_sec">
            <Card1 :mapArr="data" />
        </div>
    </div>
</template>
  
<script>
import { sec4Arr } from '../../arrays/array.js';
import Card1 from '@/components/molecules/Sec1card.vue';
import H2 from "@/components/atoms/H2.vue";

export default {
    name: "BottomSec2",
    components: {
        Card1,
        H2
    },
    data() {
        return {
            myTitle: 'MARKETPLACE',
            data: sec4Arr
        }
    }
}
</script>
  
<style>
.top_main {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: 0.5rem;
}

.top_sec {
    display: flex;
    align-items: center;
    margin: auto;
    width: 97vw;
    max-width: 1150px;
    gap: 1rem;
    justify-content: space-between;
}

@media (max-width: 400px) {
    .top_sec {
        flex-direction: column;
    }
}
</style>
  
  