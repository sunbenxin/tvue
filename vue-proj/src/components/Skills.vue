<template>
  <div class="skills">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key='index'>{{index}}. {{data.skill}}</li>
      </ul>
    </div>
    <div v-bind:class="{ alert: showAlert}">,W</div>
  </div>
</template>

<script>
export default {
  name: 'Skills',
  data(){
    return {
      skills:[
        {"skill":"Vue.js"},
        {"skill":"Frontend Developer"}
      ],
      showAlert: true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.alert {
  background-color: green;
  width:100%;
  height:30px;
}
</style>
