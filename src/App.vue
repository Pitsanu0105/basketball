<template>
  <div id="app">
    <bassget></bassget>
    <scoreboard :scoreleft = "scoreleft" :scoreright = "scoreright"></scoreboard>
    <leftboard :left-one = "leftOne" :left-two = "leftTwo" :left-three = "leftThree" :left-down ="leftDown" :score-left = "scoreleft"></leftboard>
    <rightboard :right-one = "rightOne" :right-two = "rightTwo" :right-three = "rightThree" :right-down ="rightDown" :score-right = "scoreright"></rightboard>
  </div>
</template>

<script>
import bassget from './components/bassget'
import scoreboard from './components/scoreboard'
import leftboard from './components/leftboard'
import rightboard from './components/rightboard'

export default {
  data () {
    return {
      scoreleft: 0,
      scoreright: 0
    }
  },
  components: {
    bassget,
    leftboard,
    rightboard,
    scoreboard
  },
  methods: {
    leftOne: function () {
      this.scoreleft = this.scoreleft + 1
    },
    leftTwo: function () {
      this.scoreleft = this.scoreleft + 2
    },
    leftThree: function () {
      this.scoreleft = this.scoreleft + 3
    },
    leftDown: function () {
      if (this.scoreleft > 0) {
        this.scoreleft = this.scoreleft - 1
      } else {
        this.scoreleft = 0
      }
    },
    rightOne: function () {
      this.scoreright = this.scoreright + 1
    },
    rightTwo: function () {
      this.scoreright = this.scoreright + 2
    },
    rightThree: function () {
      this.scoreright = this.scoreright + 3
    },
    rightDown: function () {
      if (this.scoreright > 0) {
        this.scoreright = this.scoreright - 1
      } else {
        this.scoreright = 0
      }
    }

  }
}

</script>

<style>
html {
  height: 100%;
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
}

#app {
  color: #2c3e50;
  margin-top: -100px;
  max-width: 600px;
  font-family: Source Sans Pro, Helvetica, sans-serif;
  text-align: center;
}

#app a {
  color: #42b983;
  text-decoration: none;
}

.logo {
  width: 100px;
  height: 100px
}
</style>
