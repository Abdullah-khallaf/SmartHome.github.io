<template>
  <div class="Notifi">
    <div class="cir">
      <img src="@/assets/imgs/warning.png" alt="warning" id="" v-for="Temp in TempData" :key="Temp.id" v-show="Temp.bill == true"/>
    </div>
    <img src="@/assets/imgs/bell.png" class="notifyimg" alt="Thermometer"> 
  </div>
</template>
<script>
import Data from "@/json/Data.json";
export default {
    data:function(){
        return{
            TempData: Data
        }
    },
   
  name: "notification"
};
</script>
<style lang="scss" scoped>
.Notifi {
  position: relative;
  .cir {
    img {
      width: 60px;
      height: 60px;
      position: absolute;
      left: 135px;
      
    }
    
  }
}

.notifyimg{
  width: 200px;
}
</style>
