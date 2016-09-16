<template>
  <div>
  <table border="3">
    <tr>
      <td width = 290px height = 300px>
        <button class="button" @click="rightOne"> +1 </button>
        <button class="button" @click="rightTwo"> +2 </button>
        <button class="button" @click="rightThree"> +3 </button>
        <button class="button" @click="rightDown" > -1 </button>
      </td>
    </tr>
  </table>
</div>
</template>

<script>
export default {
  props: ['rightOne', 'rightTwo', 'rightThree', 'rightDown', 'scoreright']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
.button {
    background-color: #FF3399;
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
div {
  display: inline;
}
</style>
