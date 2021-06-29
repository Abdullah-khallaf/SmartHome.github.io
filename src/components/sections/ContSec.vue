<template>
  <div class="ContSec">
    <b-container>
      <b-row>
        <b-col>
          <h2>
            Controllers
          </h2>
        </b-col>
      </b-row>

      <b-row class="container">
        <b-col>
          <h3>Leds</h3>
          <b-row>
            <b-col>
              <h4>Inside</h4>
              <label for="Led1">Led 1</label><toggle-button id="Led1" /><br />
              <label for="Led2">Led 2</label><toggle-button id="Led2" /><br />
              <label for="Led3">Led 3</label><toggle-button id="Led3" /><br />
              <label for="Led4">Led 4</label><toggle-button id="Led4" /><br />
              <label for="Led5">Led 5</label><toggle-button id="Led5" /><br />
            </b-col>
            <b-col>
              <h3>Outside</h3>
              <label for="LedOut1">Led 1</label
              ><toggle-button id="LedOut1" /><br />
              <label for="LedOut2">Led 2</label
              ><toggle-button id="LedOut2" /><br />
            </b-col>
          </b-row>
        </b-col>
        <b-col >
          <h3>Door</h3> <br/>
        <label for="open">OPEN</label><toggle-button id="open" /> <br/>
        <label for="close">CLOSE</label><toggle-button id="close" />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import ToggleButton from "./InnerSection/ToggleButton.vue";

export default {
  data: function() {
    return {};
  },
  name: "ContSec",
  components: {
    ToggleButton,
  },
};
</script>

<style lang="scss" scoped>
.ContSec {
  margin-top: 1%;
  height: 100%;
  background-color: #9ac7da;
  box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
}
h2 {
  margin-top: 1%;
  font-family: sans-serif;
  font-weight: bold;
  font-size: 27px;
  color: #1c3659;
  text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.705) (0, 0, 0, 0.705)
    (0, 0, 0, 0.973);
  &:hover {
    color: #0b1f3a;
  }
}
h3 {
  font-family: sans-serif;
  font-weight: bold;
  font-size: 24px;
  text-align: center;
  color: #1c3659;
  text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.705) (0, 0, 0, 0.705)
    (0, 0, 0, 0.973);
  &:hover {
    color: #0b1f3a;
  }
}
h4 {
  font-family: sans-serif;
  font-weight: bold;
  font-size: 22px;
  text-align: center;
  color: #1c3659;
  text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.705) (0, 0, 0, 0.705)
    (0, 0, 0, 0.973);
  &:hover {
    color: #0b1f3a;
  }
}
.b-container {
  .b-row {
    .b-col {
      text-align: center;
      
    }
  }
}
label {
  font-family: sans-serif;
  font-size: 25px;
  font-weight: bold;
  color: #1c3659;
  line-height: 30px;
  height: 30px;
  text-align: center;
  text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.3);
}
</style>
