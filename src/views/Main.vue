<template>
  <!-- Content -->
  <div class="neoh_fn_content">

    <!-- Hero Header -->
    <div class="neoh_fn_hero">

      <!-- Overlay (of hero header) -->
      <div class="bg_overlay">

        <!-- Overlay Color -->
        <div class="bg_color"></div>
        <!-- !Overlay Color -->

        <!-- Overlay Image -->
        <div class="bg_image" data-bg-img="/img/hero/bg.jpg"></div>
        <!-- !Overlay Image -->

      </div>
      <!-- Overlay (of hero header) -->

      <div class="hero_content">
        <div class="container">
          <div class="content">
            <h2 class="fn_title" style="font-size: calc(16px + 4vw)" title="Maxvel">Maxvel</h2>
            <p class="fn_desc fn_animated_text">Hi! I'm Max. Nice to meet you.</p>
          </div>
        </div>
        <a href="#about" class="neoh_fn_down magic-hover magic-hover__square">
          <span class="text">Scroll Down</span>
          <span class="icon"><img src="/svg/right-arr.svg" alt="" class="fn__svg"></span>
        </a>
      </div>


    </div>
    <!-- !Hero Header -->

    <AboutComponent></AboutComponent>

    <RecentWorkComponent></RecentWorkComponent>

    <CodeLangComponent></CodeLangComponent>


  </div>
  <!-- Content -->
</template>

<script>
import RecentWorkComponent from "@/views/layouts/RecentWorkComponent.vue";
import CodeLangComponent from "@/views/layouts/CodeLangComponent.vue";
import AboutComponent from "@/views/layouts/AboutComponent.vue";

export default {
  name: "Main",
  components: {AboutComponent, CodeLangComponent, RecentWorkComponent},
}
</script>

<style scoped>

</style>