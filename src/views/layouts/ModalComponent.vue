<template>
  <!-- Product Modal -->
  <div class="neoh_fn_modal product_modal">
    <div class="modal_in">
      <div class="modal_content">
        <div class="neoh_fn_product_modal">
          <div class="img_item">
            <!-- here comes product's image -->
          </div>
          <div class="content_item">
            <div class="neoh_fn_title" data-align="left">
              <h3 class="fn_title"><!-- here comes product's title --></h3>
              <div class="line"><span></span></div>
            </div>
            <div class="description" v-html="description"></div>
              <span class="text">Links:</span>
              <a href="" target="_blank" class="opensea">
                <span style="padding: 10px;color: white">link site</span>
              </a>
              <a href="" target="_blank" class="discord">
                <span style="padding: 10px;color: white">link
                  <i class="fn-icon-github"></i>
                </span>
              </a>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- !Product Modal -->
</template>

<script>
export default {
  name: "ModalComponent",
  props: {
    description: {
      default: ''
    },
  },
}
</script>

<style scoped>
.description {
  font-weight: 700;
  margin-bottom: 37px;
  margin-top: -57px;
}
</style>