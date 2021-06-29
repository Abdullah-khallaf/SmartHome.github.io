<template>
  <div class="TempSec">
    <b-container>
      <b-row>
        <b-col>
          <h2>
            Temperature
          </h2>
        </b-col>
      </b-row>

      <b-row class="container">
        <b-col>
          <toggle-button id="AutoTemp" />
          <label for="AutoTemp">Auto</label> <br />
          <range-slider id="Fan1" /><label for="Fan1"> Fan 1</label>
          <range-slider id="Fan2" /><label for="Fan2"> Fan 2</label>
          <range-slider id="Fan3" /><label for="Fan3"> Fan 3</label>
          <range-slider id="Heater1" /><label for="Heater1"> Heater 1</label>
          <range-slider id="Heater2" /><label for="Heater2"> Heater 2</label>
          <range-slider id="Heater3" /><label for="Heater3"> Heater 3</label>
        </b-col>
        <b-col>
          <temperature :Temperature="TakeTemp" />
        </b-col>
        <b-col>
          <humadity :Humadity="TakeHumid" />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>
<script>
import Humadity from './InnerSection/Humadity.vue';
import RangeSlider from "./InnerSection/RangeSlider.vue";
import Temperature from './InnerSection/Temperature.vue';
import ToggleButton from "./InnerSection/ToggleButton.vue";
import Data from "@/json/Data.json"
export default {
  data:function(){
    
    return{
      DataTemp : Data,
      TakeTemp: 10,
      TakeHumid: 20,
    }
    
  },
 
  name: "TempSection",
  components: {
    ToggleButton,
    RangeSlider,
    Temperature,
    Humadity
  },
};
</script>
<style lang="scss" scoped>
.TempSec {
  margin-top: 1%;
  background-color: #9ac7da;
  box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
}
h2 {
  margin-top: 1%;
  margin-bottom: 2%;
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
.b-container {
  .b-row {
    .b-col {
      text-align: center;
    }
  }
}
label {
  display: inline-block;
  font-family: sans-serif;
  font-size: 25px;
  font-weight: bold;
  color: #1C3659;
  text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.3);
  line-height: 30px;
  text-align: center;
  margin-left: 4px;
  height: 30px;
}
</style>
