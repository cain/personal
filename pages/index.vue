<template>
  <section class="container">
      <div class="logo">
        c h
      </div>
      <p class="sub-title">
          Extremely quick and continuous learner for modern development applications. It is my passion to deliver creative and powerful front-end applications, specialising in <a href="https://reactjs.org/">React</a> and <a href="https://vuejs.org/">Vue</a> Development.
      </p>
      <div class="section-nav">
        <a href="https://github.com/cain">code</a>        
        <a href="https://www.linkedin.com/in/cainhall/">linkedin</a>
        <a href="https://twitter.com/caintimothyhall">twitter</a>
      </div>
  </section>
</template>

<script>

export default {

}
</script>

<style>
body {
  max-height: 100vh;  
}
.container {
  display: flex;
  flex-direction: row;
  max-width: 900px;
  margin: auto;
  height: 100vh;
  justify-content: center;
  align-content: center;
  flex-direction: column;
  overflow: hidden;
}


.logo {
    background: black;
    color: #fff;
    font-weight: bold;
    font-family: "Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","\5FAE\8F6F\96C5\9ED1",Arial,sans-serif;
    width: 20px;
    text-align: center;
    height: 50px;
    margin: 60px auto;
}

.section-nav {
  margin-top: 18px;  
}

.section-nav a { 
  margin-right: 30px;
  font-size: 16px;
  font-weight: 500;
  text-align: left;
  color: #222222;
  margin: 6px 0px;
  position: relative;
  margin-right: 18px;
  transition-duration: 0.2s;
}
.section-nav a:hover {
  border-bottom: 3px solid black;
}

.sub-title {
  font-size: 14px;
  text-align: left;
  color: #222222;
  margin-top: 12px;
  font-family: "Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","\5FAE\8F6F\96C5\9ED1",Arial,sans-serif;  
}

.sub-title a {
  font-weight: bold;
  border-bottom: 3px solid black;
  text-decoration: none;
}

</style>
