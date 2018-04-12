<template>
  <section class="container">
    <div class="side m-t-120">
      <div class="banner-image">
        <div class="arrow-up"></div>
        <div class="line line-1" style="width:60px"></div>
        <div class="line line-2" style="width:60px"></div>      
        <img src="/me.png" alt="me" class="" height="250px">        
      </div>
      <div class="section-nav">
        <a href="https://github.com/cainhall">code</a>        
        <a href="https://www.linkedin.com/in/cainhall/">linkedin</a>
        <a href="https://twitter.com/caintimothyhall">twitter</a>
        <a href="mailto:cain.hall98@gmail.com">contact</a>
      </div>
    </div>
    <div class="main m-t-120">
      <div class="section-banner">
        <div class="">
          <h1 class="title text-right">
            Cain Hall
          </h1>
          <div class="line w40 m-l-a"></div>
          <p class="sub-title">
            Extremely quick and continuous learner for modern development applications. It is my passion to deliver creative and powerful front-end applications, specialising in React Development.
          </p>
        </div>
      </div>
      <!-- <div class="m-t-120">
        <h1 class="title">
          My Projects 
        </h1>
      </div> -->
    </div>
  </section>
</template>

<script>

export default {

}
</script>

<style>
.site-link {
  font-size: 14px;
  font-family: Georgia;
  margin-top: 50px;  
  text-align: right;
}
.triangle {
  position: absolute;
  top: 200px;
  left: 80px;
}
.line {
  height: 1px;
  width: 1px;
  background: black;
}

.line-1 {
  transform: rotate(140deg);
  position: absolute; 
  bottom:60px;
  left: -5px;
}

.line-2 {
  transform: rotate(140deg);
  position: absolute; 
  bottom:45px;
  left: -10px;
}

.arrow-up {
  width: 0; 
  height: 0; 
  border-left: 100px solid transparent;
  border-right: 100px solid transparent;
  
  border-bottom: 150px solid #fff;
  position: absolute;
  left: -140px;
  bottom: 0px;
}

.m-l-a { 
  margin-left: auto;
}
.m-r-a { 
  margin-right: auto;
}

.m-t-120 {
  margin-top: 100px;
}
.w40 {
  width: 40%;
}
.banner-image {
  margin-right: 12px;
  position: relative;
}
.container {
  display: flex;
  flex-direction: row;
  max-width: 900px;
  margin: auto;
}

.section-nav {
  text-align: left;
  margin-top: 24px;
  position: sticky;
  display: flex;
  flex-direction: column;
}
.section-nav a { 
  margin-right: 30px;
  font-size: 14px;
  font-weight: 500;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: left;
  color: #222222;
  margin: 6px 0px;
}
.section-banner {
  display: flex;
  flex-direction: row;
  margin-top: 100px;
  position: relative;
}

.sub-title {
  font-family: "Source Code Pro", "monaco", "PT Mono", "Courier", monospace;
  font-size: 12px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: left;
  color: #222222;
}

.title {
  font-family: Georgia;
  font-size: 40px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: left;
  color: #222222;
  margin: 6px 12px;
}

.text-right {
  text-align: right;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
