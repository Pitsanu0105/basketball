<template>
  <div style="float:left">
    <table border="3">
      <tr>
        <td width = 285px height = 300px >
          <button class="button" @click="leftOne"> +1 </button>
          <button class="button" @click="leftTwo"> +2 </button>
          <button class="button" @click="leftThree"> +3 </button>
          <button class="button" @click="leftDown"> -1 </button>
        </td>
      </tr>
  </table>
  </div>

</template>

<script>
export default {
  props: ['leftOne', 'leftTwo', 'leftThree', 'leftDown', 'scoreleft']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
.button {
    background-color: #4CAF50;
    border: none;
    color: white;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    cursor: pointer;
    width: 50px;
    height: 50px;
    font-size: 20px;
}
</style>
