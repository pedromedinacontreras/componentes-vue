<template>
  <b-row align-h="start" align-v="center" >
    <b-col cols=".7" style="font-weight: bold;cursor:pointer;color:grey" @click="onBack">
      <h5 style="font-size:20px;" class='material-icons align-bottom'>arrow_back</h5>
    </b-col>
    <b-col cols=".7" style="cursor:pointer;color:grey" @click="onBack">
      <h5 style="font-size:14px;padding-left:3px;">Volver</h5>
    </b-col>
    <b-col>
      <h3 style="padding-left:20px;">{{ title }}</h3>
    </b-col>
  </b-row>
</template>

<script>
export default {
  props: {
    title: { type: String },
  },
  methods: {
    onBack() {
      this.$router.go(-1);
    },
  },
}
</script>

<style lang="css" scoped>
</style>
