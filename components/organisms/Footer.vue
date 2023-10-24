<template>
  <div class="footer_sec">
    <H2 :heading="title" />
    <Pfooter :text="p1" :span="span" />
    <Pfooter :text="p2" :span="span" />
    <Pfooter :text="p3" :span="span" />
    <Pfooter :text="p4" :span="span" />
  </div>
</template>

<script>
import Pfooter from '../atoms/Pfooter.vue';
import H2 from '../atoms/H2.vue';
export default {
  name: "Footer",
  components: {
    H2,
    Pfooter
  },
  data() {
    return {
      title: "ACCOUNT MANAGEMENT",
      p1: "Add Existing Admin User to Additional Account -",
      p2: "Add Support Staff to Member's Area -",
      p3: "Need to Pause Your Account -",
      p4: "Want to Cancel Your Account -",
      span: "CLICK HERE",
    }
  }
}
</script>

<style>
.footer_sec {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  text-align: left;
  width: 97vw;
  max-width: 1150px;
  margin: auto;
}
</style>
