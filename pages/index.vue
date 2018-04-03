<template>
  <section class="container">
    <div class="section-nav">
      <a href="#">home</a>
      <a href="#">work</a>
      <a href="#">blog</a>
      <a href="#">contact</a>
    </div>
    <div class="section-banner">
      <h1 class="title">
        Something Cool Here
      </h1>
      <p class="sub-title">
        Tumblr polaroid DIY tilde green juice bicycle rights. Farm-to-table vape lo-fi tote bag literally salvia. Taiyaki gluten-free roof party aesthetic slow-carb swag banh mi gentrify cronut bicycle rights. Green juice whatever microdosing shoreditch, tote bag slow-carb jianbing hashtag gentrify swag photo booth edison bulb.
      </p>
    </div>
  </section>
</template>

<script>

export default {

}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  text-align: center;
  flex-direction: column;
  max-width: 1000px;
  margin: auto;
}

.section-nav {
  text-align: left;
  margin-top: 6px;
  position: fixed;
}
.section-nav a { 
  margin-right: 30px;
  font-family: LucidaGrande;
  font-size: 14px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: left;
  color: #222222;
}
.section-banner {
  height: 100vh;
  display: flex;
  flex-direction: column;
  margin-top: 30vh;
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
  margin: 12px 0px;
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
