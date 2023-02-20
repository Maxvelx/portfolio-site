<template>
  <!-- Main -->
  <div class="neoh_fn_main bg-main" data-footer-sticky="">

    <!-- Right Navigation -->
    <div class="nav_overlay"></div>
    <div class="neoh_fn_nav">
      <div class="trigger is-active">
        <div class="trigger_in">
          <span class="text">Close</span>
          <span class="hamb">
					<span class="hamb_a"></span>
					<span class="hamb_b"></span>
					<span class="hamb_c"></span>
				</span>
        </div>
      </div>
      <div class="nav_content">
        <div class="nav_menu">
          <ul>
            <li class="menu-item"><a href="/">Home</a></li>
            <li class="menu-item"><a href="#about">About Me</a></li>
            <li class="menu-item"><a href="#drop">Recent work</a></li>
            <li class="menu-item"><a href="#investor">Skills</a></li>
            <li class="menu-item"><a href="#footer">Contact</a></li>
          </ul>
        </div>
        <div class="nav_buttons">
          <a href="https://github.com/Maxvelx" class="neoh_fn_button"
             target="_blank" rel="noopener noreferrer">
            <span class="icon"><i class="fn-icon-github-1"></i></span>
            <span class="text">Github</span>
          </a>
          <a href="https://www.linkedin.com/in/max-ivanchenko-534205267/" class="neoh_fn_button">
            <span class="icon"><i class="fn-icon-linkedin-1"></i></span>
            <span class="text">Linked-In</span>
          </a>
        </div>
      </div>

      <!-- Nav Footer -->
      <div class="nav_footer">
        <div class="nf_left">
          <p>🗸 Maxvel</p>
        </div>
        <div class="nf_right">
          <div class="neoh_fn_social_list">
            <ul>
              <li>
                <a href="https://t.me/maxvelx1" target="_blank" rel="noopener noreferrer">
                <i class="fn-icon-telegram"></i>
              </a>
              </li>
              <li>
                <a href="mailto:maxvelx.develop@gmail.com" target="_blank" rel="noopener noreferrer">
                <i class="fn-icon-email"></i>
              </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <!-- !Nav Footer -->

    </div>
    <!-- !Right Navigation -->

    <!-- Header -->
    <header class="neoh_fn_header">
      <div class="container">
        <div class="header_in">

          <div class="logo" style="width: 60px;height: 60px;">
            <a style="aspect-ratio: 3/2;object-fit: contain;"
               href="/"><img src="/img/logo.jpg" alt=""></a>
          </div>

          <div class="trigger">
            <div class="trigger_in">
              <span class="text">Menu</span>
              <span class="hamb">
							<span class="hamb_a"></span>
							<span class="hamb_b"></span>
							<span class="hamb_c"></span>
						</span>
            </div>
          </div>

        </div>
      </div>
    </header>
    <!-- !Header -->

    <Main></Main>

    <FooterComponent></FooterComponent>

    <!-- Totop -->
    <a href="#" class="neoh_fn_totop">
      <span class="arrow"><img src="/svg/right-arr.svg" alt="" class="fn__svg"></span>
      <span class="circle"><img src="/svg/circle.svg" alt="" class="fn__svg"></span>
    </a>
    <!-- !Totop -->


  </div>
  <!-- !Main -->
</template>

<script setup>
import FooterComponent from "@/views/layouts/FooterComponent.vue";
import Main from "@/views/Main.vue";

</script>

<style scoped>

</style>
