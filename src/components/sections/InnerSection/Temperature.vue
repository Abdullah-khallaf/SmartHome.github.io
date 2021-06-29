<template>
  <div>
    <h2>Temperature</h2>
    <p>{{ Temperature }}<span>deg</span></p>
  </div>
</template>
<script>
export default {
  props:["Temperature"],
  name:"Temperature",
  
};
</script>
<style lang="scss" scoped>
h2{
  margin-top: 1%;
  text-align: center;
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

p {
  font-family: sans-serif;
  font-size: 180px;
  font-weight: bold;
  color: #1c3659;
  text-align: center;
  text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.3);
  position: relative;
  span {
    position: absolute;
    top: 30px;
    left: 80%;
    font-family: sans-serif;
    font-size: 25px;
    font-weight: bold;
    color: #1c3659;
    text-align: center;
    text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.3);
  }
}
</style>
