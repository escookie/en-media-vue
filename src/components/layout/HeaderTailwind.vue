<template>
    <header class="bg-white">
      <nav class="mx-auto max-w-7xl items-center justify-between p-6 lg:px-8 header-flex" aria-label="Global">
        <div class="flex lg:flex-1 justify-between lg:justify-start">
          <a href="#" class="-m-1.5 p-1.5">
            <img class="h-8 w-auto" src="../../assets/logo.svg" alt="" @click="handleClick('Home')"/>
          </a>
          <!-- 모바일 네비게이션 버튼 -->
          <div class="flex lg:hidden justify-end">
            <button type="button" class="p-1.5" @click="mobileMenuOpen = !mobileMenuOpen">
              <span class="sr-only">Open main menu</span>
              <i class="fa-solid fa-bars"></i>
            </button>
          </div>
        </div>
        <!-- 드롭다운 메뉴 -->
        <PopoverGroup class="hidden lg:flex lg:gap-x-12 justify-end">
          <a href="#" class="text-sm font-semibold leading-6 text-gray-900" @click="handleClick('Home')">Home</a>
          <a href="#" class="text-sm font-semibold leading-6 text-gray-900" @click="handleClick('About')">About</a>
          <a href="#" class="text-sm font-semibold leading-6 text-gray-900" @click="handleClick('Contact')">Contact</a>
        </PopoverGroup>
        
        

        <!-- 모바일 메뉴 -->
        <div :style="mobileMenuOpen ? 'max-height: 200px; opacity: 1; padding-top: 20px;' : 'max-height: 0; opacity: 0; padding-top: 0'" 
          class="overflow-hidden transition-all duration-300 hamburger-mobile-menu">
          <a href="#" class="block text-sm font-semibold leading-6 text-gray-900" @click="handleClick('Home')">Home</a>
          <a href="#" class="block text-sm font-semibold leading-6 text-gray-900" @click="handleClick('About')">About</a>
          <a href="#" class="block text-sm font-semibold leading-6 text-gray-900" @click="handleClick('Contact')">Contact</a>
        </div>

        
      </nav>
    </header>
</template>

  
  <script>
  export default {
      data() {
          return {
              mobileMenuOpen: false
          };
      },
      methods: {
          handleClick(page) {
              console.log(`${page} 클릭`);
          }
      }
  }
  </script>

<style>
i{color: black;}
.header-flex{
  display: flex;
}
.hamburger-mobile-menu{display: none;}
@media screen and (max-width:600px) {
  .header-flex{display: block;}
  .hamburger-mobile-menu{display: block;}
}
</style>