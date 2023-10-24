<template>
  <div class="nav_sec">
    <Button :text="leftText" :time="time1">
    </Button>
    <div class="nav_mid">
      <h2 class="h1">Need More Support?</h2>
      <Ptag :text="pText" class="exp" />
      <Ptag :text="pText2" class="exp2" />
    </div>

    <Button :text="rightText" :time="time2">
    </Button>
  </div>
</template>

<script>
import Button from '../atoms/Button.vue';
import Ptag from '../atoms/Ptag.vue';
export default {
  name: "Nav",
  components: {
    Button,
    Ptag
  },
  data() {
    return {
      leftText: "Monday.Click To Join",
      time1: "7pm UK / 2pm New York",
      time2: "10am UK / 7pm Sydney",
      pText: "JOIN A LIVE GROUP COACHING SESSION",
      pText2: "Click to Register for Reminders",
      rightText: "Thursday.Click To Join",
    }
  }
}
</script>

<style>
.nav_sec {
  display: flex;
  width: 100%;
  flex-direction: row;
  background: #d9bb6aff;
  color: #000;
  padding: 0rem;
  justify-content: space-between;
  align-items: center;
}

.nav_mid {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 30vw;
  max-width: 400px;
  margin: 0 auto;
  gap: 0;
}

.h1 {
  font-size: 23px !important;
  font-family: Arial, Helvetica, sans-serif;
  font-weight: 700;
  margin-bottom: 0;
  text-align: center;
}

.exp {
  font-size: 20px;
  font-weight: 0;
  margin: 0 auto;
}

.exp2 {
  font-size: 16px;
  font-weight: 0;
  margin: 0 auto 1rem;
}

.exp:hover,
.exp2:hover {
  text-decoration: underline;
  cursor: pointer;
}

@media (max-width: 600px) {
  .nav_sec {
    flex-direction: column;
    padding: 0rem 0.5rem;
  }

  .h1 {
    line-height: 1rem;
    margin: 1rem auto;
  }
}
</style>
