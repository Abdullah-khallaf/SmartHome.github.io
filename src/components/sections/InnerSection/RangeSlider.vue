<template>
  <div>
    <input v-model="value" type="range" class="MySlider" min="0" max="5" />
    <span class="rangeValue"> {{ value }} </span>
  </div>
</template>
<script>
export default {
    data:function(){
        return{
            value: 0
        }
    },
  name: "RangeSlider",
};
</script>
<style lang="scss" scoped>
div{
    padding-bottom: 10px;
    display: inline-block;
}
.MySlider {
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  width: 180px;
  height: 30px;
  margin-right: 5px;
  background-color: #3370a6;
  border-radius: 50px;
  opacity: 0.9;
  transition: opacity 0.1s ease-in;
  cursor: pointer;
  &:hover {
    opacity: 1;
  }
  &::-webkit-slider-thumb {
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
    height: 33px;
    width: 33px;
    background-color: #ffffff;
    border-radius: 50px;
    cursor: pointer;
  }
  
}
.rangeValue{
    font-family: sans-serif;
    font-size: 25px;
    font-weight: bold;
    color: #1C3659;
    line-height: 30px;
    height: 30px;
    text-align: center;
    text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.3);
    
    
  }
</style>
