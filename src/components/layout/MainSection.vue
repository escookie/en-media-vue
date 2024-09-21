<template>
    <div id="default-carousel" class="relative w-full carousel-padding" data-carousel="slide">
      <!-- Carousel wrapper -->
      <div class="relative h-56 overflow-hidden rounded-lg md:h-96">
        <!-- Item 1 -->
        <div class="hidden duration-700 ease-in-out" data-carousel-item>
          <div class="relative w-full h-full">
            <img src="../../assets/images/main.jpg" class="absolute block w-full h-full object-cover" alt="...">
            <div class="absolute inset-0 flex items-center justify-center flex-col carousel-item-padding">
              <p class="text-white bg-opacity-50 p-2 text-5xl text-shadow-main mobile-text-1">Lorem ipsum dolor sit amet,</p>
              <p class="text-white bg-opacity-50 text-shadow">Lorem ipsum dolor sit amet, consectetur sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
            </div>
          </div>
        </div>
        <!-- Item 2 -->
        <div class="hidden duration-700 ease-in-out" data-carousel-item>
          <div class="relative w-full h-full">
            <img src="../../assets/images/img1.jpg" class="absolute block w-full h-full object-cover" alt="...">
            <div class="absolute inset-0 flex items-center justify-center flex-col carousel-item-padding">
              <p class="text-white bg-opacity-50 p-2 text-5xl text-shadow-main mobile-text-1">Lorem ipsum dolor sit amet,</p>
              <p class="text-white bg-opacity-50 text-shadow">Lorem ipsum dolor sit amet, consectetur sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
            </div>
          </div>
        </div>
        <!-- Item 3 -->
        <div class="hidden duration-700 ease-in-out" data-carousel-item>
          <div class="relative w-full h-full">
            <img src="../../assets/images/img2.jpg" class="absolute block w-full h-full object-cover" alt="...">
            <div class="absolute inset-0 flex items-center justify-center flex-col carousel-item-padding">
              <p class="text-white bg-opacity-50 p-2 text-5xl text-shadow-main mobile-text-1">Lorem ipsum dolor sit amet,</p>
              <p class="text-white bg-opacity-50 text-shadow">Lorem ipsum dolor sit amet, consectetur sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
            </div>
          </div>
        </div>
        <!-- Item 4 -->
        <div class="hidden duration-700 ease-in-out" data-carousel-item>
          <div class="relative w-full h-full">
            <img src="../../assets/images/img3.jpg" class="absolute block w-full h-full object-cover" alt="...">
            <div class="absolute inset-0 flex items-center justify-center flex-col carousel-item-padding">
              <p class="text-white bg-opacity-50 p-2 text-5xl text-shadow-main mobile-text-1">Lorem ipsum dolor sit amet,</p>
              <p class="text-white bg-opacity-50 text-shadow">Lorem ipsum dolor sit amet, consectetur sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
            </div>
          </div>
        </div>
      </div>
      <!-- Slider indicators and controls -->
      <div class="absolute z-30 flex -translate-x-1/2 bottom-5 left-1/2 space-x-3 rtl:space-x-reverse">
        <button type="button" class="w-3 h-3 rounded-full" aria-current="true" aria-label="Slide 1" data-carousel-slide-to="0"></button>
        <button type="button" class="w-3 h-3 rounded-full" aria-current="false" aria-label="Slide 2" data-carousel-slide-to="1"></button>
        <button type="button" class="w-3 h-3 rounded-full" aria-current="false" aria-label="Slide 3" data-carousel-slide-to="2"></button>
        <button type="button" class="w-3 h-3 rounded-full" aria-current="false" aria-label="Slide 4" data-carousel-slide-to="3"></button>
      </div>
      <button type="button" class="absolute top-0 start-0 z-30 flex items-center justify-center h-full px-4 cursor-pointer group focus:outline-none button-padding" data-carousel-prev style="padding-left: 7%;">
        <span class="inline-flex items-center justify-center w-10 h-10 rounded-full bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none responsive-circle">
          <svg class="w-4 h-4 text-white dark:text-gray-800 rtl:rotate-180 responsive-svg" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 6 10">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 1 1 5l4 4"/>
          </svg>
          <span class="sr-only">Previous</span>
        </span>
      </button>
      <button type="button" class="absolute top-0 end-0 z-30 flex items-center justify-center h-full px-4 cursor-pointer group focus:outline-none button-padding" data-carousel-next>
        <span class="inline-flex items-center justify-center w-10 h-10 rounded-full bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none responsive-circle">
          <svg class="w-4 h-4 text-white dark:text-gray-800 rtl:rotate-180 responsive-svg" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 6 10">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 9 4-4-4-4"/>
          </svg>
          <span class="sr-only">Next</span>
        </span>
      </button>
    </div>    
  </template>
  
<script>
export default {
  name: 'MainSection',
};
</script>

<style scoped>
.text-shadow-main {
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
  }
.text-shadow {
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.4);
}

@media screen and (max-width:600px) {
  .carousel-padding{padding: 2% 7%;}
  .mobile-text-1{font-size: 1.5rem;}
  .carousel-item-padding{padding: 5% 10%}

  .responsive-svg{
    width: 1rem; 
    height: 1rem;
  }
  .responsive-circle{
    width: 2rem; 
    height: 2rem;
    margin: 5px;    
  }
  .button-padding{
    padding: 7% ;
  }
}
</style>