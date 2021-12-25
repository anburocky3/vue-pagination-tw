<script lang="ts">
import { defineComponent } from 'vue';
import VuePaginationTw from '@/components/vue-pagination-tw.vue';
import "../src/assets/styles/tailwind.css"

export default defineComponent({
  name: 'ServeDev',
  components: {
    VuePaginationTw
  },
  data() {
    return {
      customClass: {
        'ul': 'ad'
      }
    }
  },
  mounted() {
    let externalScript = document.createElement('script')
    externalScript.setAttribute('src', 'https://cdn.tailwindcss.com')
    document.head.appendChild(externalScript)
  }
});
</script>

<template>
  <div id="app" class="min-h-screen bg-gray-200 flex items-center">
    <div class="container mx-auto bg-white rounded shadow-sm p-10">
      <div class="text-center">
        <vue-pagination-tw
          :total-items="20"
          :current-page="1"
          :per-page="6"
          @page-changed="console.log('s')"
          :go-button="false"
          borderActiveColor="border-red-500"
          borderTextActiveColor="text-red-500"
        />
      </div>
    </div>
  </div>
</template>


<style scoped>
</style>