<template>
  <div>
    <label class="switch">
      <input type="checkbox" unchecked/>
      <div class="switch-btn"></div>
    </label>
  </div>
</template>
<script>
export default {
  name: "toggleButton",
};
</script>
<style lang="scss" scoped>
div{
  display: inline-block;
  }
input[type="checkbox"] {
  opacity: 0;
}
.switch-btn {
  width: 60px;
  height: 30px;
  background-color: #3370a6;
  position: relative;
  border-radius: 50px;
  cursor: pointer;
  opacity: .9;
  transition: opacit .1s ease-in;
  &:hover{
    opacity: 1;
  }
}
.switch-btn:before {
  content: " ";
  position: absolute;
  height: 30px;
  width: 30px;
  background-color: #ffffff;
  border-radius: 50px;
  left: 0px;
  top: 0px;
  transition: 150ms ease-out;
}
input[type="checkbox"]:checked + .switch-btn:before {
  left: 30px;
}

input[type="checkbox"]:checked + .switch-btn{
  background-color: #33A661;
}
</style>
