<template>
  <section class="container">
    <a class="site-link" href="#">cainhall.com.au</a>
    <div class="section-banner">
      <img src="/me.jpg" alt="me" class="banner-image" height="300px">
      <div>
        <h1 class="title">
          Some Random Title
        </h1>
        <div class="line w40"></div>
        <p class="sub-title">
          Tumblr polaroid DIY tilde green juice bicycle rights. Farm-to-table vape lo-fi tote bag literally salvia. Taiyaki gluten-free roof party aesthetic slow-carb swag banh mi gentrify cronut bicycle rights. Green juice whatever microdosing shoreditch, tote bag slow-carb jianbing hashtag gentrify swag photo booth edison bulb.
        </p>
      </div>
    </div>
    <div class="section-nav">
      <a href="#">home</a>
      <a href="#">projects</a>
      <a href="#">blog</a>
      <a href="#">contact</a>
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
  margin-left: auto;
}
.w40 {
  width: 40%;
}
.banner-image {
  margin-right: 12px;
}
.container {
  min-height: 400vh;
  display: flex;
  flex-direction: column;
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
  text-align: right;
  color: #222222;
  margin: 6px 12px;
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
