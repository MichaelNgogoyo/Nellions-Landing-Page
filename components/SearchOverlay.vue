<template>
  <div>
    <div @click="showSearch = true" class="cursor-pointer">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
           stroke="currentColor" class="size-6">
        <path stroke-linecap="round" stroke-linejoin="round"
              d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z"/>
      </svg>
    </div>
    <transition name="fade">
      <div v-if="showSearch" class="fixed inset-0 bg-black bg-opacity-90 flex items-center justify-center">
        <div class="absolute top-4 right-4">
          <button @click="showSearch = false" class="text-white">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"
                 xmlns="http://www.w3.org/2000/svg">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
            </svg>
          </button>
        </div>
        <input type="text" class="w-3/4 p-4 text-xl text-black bg-white rounded" placeholder="Search...">
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showSearch: false
    }
  }
}
</script>

<style>
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s;
}

.fade-enter, .fade-leave-to /* .fade-leave-active in <2.1.8 */
{
  opacity: 0;
}
</style>
