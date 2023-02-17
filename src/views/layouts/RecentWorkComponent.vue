<template>

  <!-- Recent Work Section -->
  <section id="drop">
    <div class="container">

      <!-- Main Title -->
      <div class="neoh_fn_title">
        <h3 class="fn_title">My Recent Work</h3>
        <div class="line"><span></span></div>
      </div>
      <!-- !Main Title -->


      <!-- Recent Work List -->
      <div class="neoh_fn_drops">
        <ul>
          <li>
            <div class="item" data-modal-image="/img/drops/e-shop2.jpg" data-modal-title="E-shop"
                 data-modal-description="" data-modal-discord-url="https://github.com/Maxvelx/dmv"
                 data-modal-opensea-url="https://shop.template.maxvel.pp.ua/">
              <div class="img_holder">
                <img src="/img/drops/e-shop.jpg" alt="">
                <a href="#" @click.prevent="descToHtml('one')" class="full_link"></a>
              </div>
              <div class="title_holder">
                <h3 class="fn_title"><a href="#" @click.prevent="descToHtml('one')">E-shop car spare parts | Vue 3</a>
                </h3>
              </div>
            </div>
          </li>
          <li>
            <div class="item" data-modal-image="/img/drops/admin-panel.jpg" data-modal-title="Admin Panel"
                 data-modal-description="" data-modal-discord-url="https://github.com/Maxvelx/admin.shop"
                 data-modal-opensea-url="https://adminshop.template.maxvel.pp.ua/">
              <div class="img_holder">
                <img src="/img/drops/admin-panel2.jpg" alt="">
                <a href="#" @click.prevent="descToHtml('two')" class="full_link"></a>
              </div>
              <div class="title_holder">
                <h3 class="fn_title"><a href="#" @click.prevent="descToHtml('two')">Admin Panel | Vue 3</a></h3>
              </div>
            </div>
          </li>
          <li>
            <div class="item" data-modal-image="/img/drops/apirest.png" data-modal-title="REST API"
                 data-modal-description="" data-modal-discord-url="https://github.com/Maxvelx/backend"
                 data-modal-opensea-url="https://api.template.maxvel.pp.ua/api/parts">
              <div class="img_holder">
                <img src="/img/drops/apirest1.jpg" alt="">
                <a href="#" @click.prevent="descToHtml('three')" class="full_link"></a>
              </div>
              <div class="title_holder">
                <h3 class="fn_title"><a href="#" @click.prevent="descToHtml('three')">REST API | Laravel 9+</a></h3>
              </div>
            </div>
          </li>
        </ul>

        <!-- Clearfix -->
        <div class="clearfix"></div>

        <!--        &lt;!&ndash; Main Button &ndash;&gt;-->
        <!--        <a href="" class="neoh_fn_button only_text full">-->
        <!--          <span class="text">Click here to see all my work</span>-->
        <!--        </a>-->
        <!--        &lt;!&ndash; !Main Button &ndash;&gt;-->

      </div>
      <!-- !Recent Work List -->
      <ModalComponent
          :description="descriptionModal ? descriptionModal : ''"
      />
    </div>
  </section>
  <!-- !Recent Work Section -->
</template>

<script>
import ModalComponent from "@/views/layouts/ModalComponent.vue";

export default {
  name: "RecentWorkComponent",
  components: {ModalComponent},
  data() {
    return {
      descriptionModal: {
        type: Text
      },
      descriptionArray: {
        one: 'For create used: <br> \n' +
            '<span style="color: green">Vue 3</span> with <span style="color: green">VueX</span> for overall work<br>\n' +
            '<span style="color: darkorange">Axios</span> to connect <span style="color: orangered">Laravel</span> Rest API<br>\n' +
            '<span style="color: royalblue">JWT</span> for security',
        two: 'For create used: <br> \n' +
            '<span style="color: green">Vue 3</span> with <span style="color: green">VueX</span> for overall work<br>\n' +
            '<span style="color: darkorange">Axios</span> to connect <span style="color: orangered">Laravel</span> Rest API<br>\n' +
            '<span style="color: royalblue">JWT</span> for security',
        three: 'For create used:<br> \n' +
            '<span style="color: orangered">Laravel 9+</span> for overall work<br>\n' +
            '<span style="color: royalblue">JWT</span> for security',
      }
    }
  },
  methods: {
    descToHtml(id) {
      this.descriptionModal = this.descriptionArray[id]
    }
  },
}
</script>

<style scoped>

</style>