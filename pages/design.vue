<template>
  <div class="main">
    <Nav />
    <div class="inner">
      <Topsec />
      <Middlesec />
      <Bottomsec />
      <Line />
      <BottomSec2 />
      <Line />
    </div>
    <Footer />
  </div>
</template>

<script>

import Nav from '~/components/organisms/Nav.vue'
import Topsec from '~/components/organisms/Topsec.vue';
import Middlesec from '~/components/organisms/Middlesec.vue';
import Bottomsec from '~/components/organisms/Bottomsec.vue';
import Line from '~/components/atoms/Line.vue';
import BottomSec2 from '~/components/organisms/BottomSec2.vue';
import Footer from '~/components/organisms/Footer.vue';

export default {
  name: "design",
  components: {
    Nav,
    Topsec,
    Middlesec,
    Bottomsec,
    Line,
    BottomSec2,
    Footer
  }
}

</script>



<style>
.main {
  /* width: 100vw; */
  height: fit-content;
  min-height: 100vh;
  display: flex;
  margin: 0 auto;
  flex-direction: column;
  overflow-x: hidden;
  /* background: #000; */
}

.inner {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  gap: 3rem;
  margin: 2rem auto;
}
</style>
