<template>
  <div class="NotificationSec">
    <b-container>
      <b-row>
        <b-col>
          <h2>
            Notifications
          </h2>
        </b-col>
      </b-row>

      <b-row class="container">
        <b-col>
         <temp-notify/>
        </b-col>
        <b-col>
          <alert-notify />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import AlertNotify from './InnerSection/AlertNotify.vue';
import Notification from "./InnerSection/Notification.vue";
import TempNotify from './InnerSection/TempNotify.vue';


export default {
    data: function(){
        return{
            
        }
    },
  name: "notifications",
  components: {
    Notification,
    TempNotify,
    AlertNotify,
  },
};
</script>

<style lang="scss" scoped>
.NotificationSec{
  margin-top: 1%;
  padding-bottom: 10px;
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
.b-container {
  .b-row {
    .b-col {
      text-align: center;
    }
  }
}</style>
