<template>
  <div class="Notifi">
    <div class="cir">
      <img src="@/assets/imgs/warning.png" alt="warning" id="" />
    </div>
    
  </div>
</template>
<script>
export default {
  name: "notification"
};
</script>
<style lang="scss" scoped>
.Notifi {
  position: relative;
  .cir {
    img {
      width: 50px;
      height: 50px;
      position: absolute;
      right: 120px;
    }
    
  }
}

img {
  width: 200px;
}
</style>
