<template>
  <table border="3" >
    <tr>
      <td width = 300px>
        <center>
        <div>
            <h1>Home</h1>
            <h2>{{ scoreleft }}</h2>
        </div>
        </center>
      </td>
      <td width = 300px>
        <center>
        <div>
          <h1>Away</h1>
          <h2>{{ scoreright }}</h2>
        </div>
        </center>
      </td>
    </tr>
  </table>
</template>

<script>
export default {
  props: ['scoreleft', 'scoreright']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h2 {
  color: #42b983;
  font-size: 70px;
}
h1{
  color: blue;
}
</style>
