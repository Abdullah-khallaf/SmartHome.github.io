<template>
  <div class="FooterSec">
    <b-container>
      <b-row>
        <b-col>
          <h2>
            All Copyrights 	&copy; preserved to FEE GEEKS
          </h2>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "FooterSec",
};
</script>

<style lang="scss" scoped>
.FooterSec {
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

</style>
