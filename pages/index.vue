<template>
  <section class="container">
    <h1>Cain Hall</h1>

    <div id="scene">

      <canvas height="4000" width="4000" data-depth="1"/>
    </div>
  </section>
</template>

<script>
import axios from '~/plugins/axios'
import { Button, Select } from 'element-ui'
import Parallax from 'parallax-js/dist/parallax.min.js'
export default {
  components: {
    Button, Select
  },
  async asyncData () {
    let { data } = await axios.get('/api/users')
    return { users: data }
  },
  head () {
    return {
      title: 'Users'
    }
  },
  mounted () {
    document.addEventListener('touchmove', function (e) {
      e.preventDefault()
    })
    var c = document.getElementsByTagName('canvas')[0]

    var x = c.getContext('2d')
    var pr = window.devicePixelRatio || 1
    var w = 2000
    var h = 2000
    var f = 90
    var q
    var m = Math
    var r = 0
    var u = m.PI * 2
    var v = m.cos
    var z = m.random
    c.width = w * pr
    c.height = h * pr
    x.scale(pr, pr)
    x.globalAlpha = 0.6
    function i () {
      x.clearRect(0, 0, w, h)
      q = [{x: 0, y: h * 0.7 + f}, {x: 0, y: h * 0.7 - f}]
      while (q[1].x < w + f) d(q[0], q[1])
    }
    function d (i, j) {
      x.beginPath()
      x.moveTo(i.x, i.y)
      x.lineTo(j.x, j.y)
      var k = j.x + (z() * 2 - 0.25) * f
      var n = y(j.y)
      x.lineTo(k, n)
      x.closePath()
      r -= u / -50
      x.fillStyle = '#' + (v(r) * 127 + 128 << 16 | v(r + u / 3) * 127 + 128 << 8 | v(r + u / 3 * 2) * 127 + 128).toString(16)
      x.fill()
      q[0] = q[1]
      q[1] = {x: k, y: n}
    }
    function y (p) {
      var t = p + (z() * 2 - 1.1) * f
      return (t > h || t < 0) ? y(p) : t
    }
    document.onclick = i
    document.ontouchstart = i
    i()

    var scene = document.getElementById('scene')
    var parallaxInstance = new Parallax(scene)
    parallaxInstance.friction(0.2, 0.2)
  }
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css?family=Roboto+Slab');
canvas, #scene {
    position: absolute;
    top: -40%;
    left: -40%;
    z-index: 0;
    width: 140%;
    height: 140%;
    pointer-events: none;
    overflow: hidden
}
h1 {
  font-family: 'Roboto Slab', serif;
}
</style>
