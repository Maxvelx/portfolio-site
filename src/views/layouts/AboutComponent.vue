<template>
  <!--About Me -->
  <section id="about" class="bg-border-end neoh_fn_about_item">
    <div class="container width">
      <div class="title_about">
        Hi! I'm Max.
        <br>
        I'm a web full-stack developer from Ukraine.
      </div>
      <div class="content_about">
        I've been working as a freelance developer since 2022. I have always been a person who has both creative
        and
        logical side. When I discovered web programming, I realized that it was the perfect fit for me. I'm quietly
        confident, naturally curious, and perpetually working on improving my chops.
      </div>
    </div>
    <div class="container width">
      <div class="title_about">
        I love working with small businesses
      </div>
      <div class="content_about">
        I specialize in creating websites for individuals and small businesses. I create customized websites at
        affordable prices. Your website is often the first impression your customers get, so make sure it's a good
        one. Since my time is split between several different things, I can't take on every project I'd like to, but
        I'm always looking for interesting work.
      </div>
    </div>
  </section>
  <!--!About Me -->
</template>

<script>
export default {
  name: "AboutComponent"
}
</script>

<style scoped>
.title_about {
  font-family: "Verdana";
  font-size: 24px;
  font-weight: 500;
}

.content_about {
  padding-top: 10px;
  max-width: 520px;
  font-family: "Verdana";
  font-size: 17px;
}
.width {
  width: 50%;
}
@media (max-width: 768px) {
  .width{
    padding-bottom: 50px;
    width: 95%;
  }
}

</style>