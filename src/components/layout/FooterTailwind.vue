<template>
    <footer class="bg-gray-200 w-full shadow bg-gray-100">
        <div class="w-full max-w-screen-xl mx-auto p-4 md:py-8">
            <div class="sm:flex sm:items-center sm:justify-between">
                <div class="flex items-center justify-center mb-4 sm:mb-0 space-x-3 rtl:space-x-reverse black-and-white">
                    <img src="../../assets/logo.svg" class="h-8" alt="" @click="handleClick('Home')"/>
                </div>
                <div class="footer-align">
                    <li>
                    <a href="#" class="hover:underline me-4 md:me-6" @click="handleClick('About')">About</a>
                    </li>
                    <li>
                        <a href="#" class="hover:underline me-4 md:me-6" @click="handleClick('Privacy Policy')">Privacy Policy</a>
                    </li>
                    <li>
                        <a href="#" class="hover:underline me-4 md:me-6" @click="handleClick('Licensing')">Licensing</a>
                    </li>
                    <li>
                        <a href="#" class="hover:underline" @click="handleClick('Contact')">Contact</a>
                    </li>
                    <div class="pc-copyright">
                        <span class="block text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2024 ENMEDIA™. All Rights Reserved.</span>
                    </div>
                
                </div>
                <div class="mobile-copyright">
                    <span class="block text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2024 ENMEDIA™. All Rights Reserved.</span>
                </div>
            </div>
            
        </div>
    </footer>
</template>



<script>
export default {
    methods: {
      handleClick(page) {
        console.log(`${page} 클릭`);
      }
    }
  }
</script>

<style>
.black-and-white img{
    filter: grayscale(100%);
    opacity: 0.7;
}
.mobile-copyright{display: none}
.footer-align{display: flex; list-style: none; font-size: 0.9rem; justify-content: center;}
.pc-copyright{padding-left: 40px;}

@media screen and (max-width:600px) {
    .black-and-white {padding-top: 5px;}
    .mobile-copyright{display: block; padding-top: 35px}
    .pc-copyright{display: none;}
}
</style>

