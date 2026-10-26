<script setup lang="ts">
import LogoSimpsons from '@/components/LogoSimpsons.vue';


</script>

<template>
    <div class="grid grid-rows-[auto_1fr_auto] min-h-screen">

        <header class="bg-simpsons-yellow w-full border border-black">

            <div class="flex flex-col items-center md:flex-row justify-between p-3 md:px-20 mx-auto max-w-page">

            <LogoSimpsons estilus="w-[8rem] h-auto" />

            <div class="flex gap-6 pt-3">
           <RouterLink 
           to="/simpsons/gallery"
           active-class="font-bold"
           
           >
            Characters
          </RouterLink>

          <RouterLink to="/simpsons/about"
          active-class="font-bold"
          >
            About
          </RouterLink>

          <Button class="bg-white text-base border border-black hover:bg-simpsons-red focus:bg-simpsons-red rounded-none text-black h-7.5 py-0.5 px-5">
      		<RouterLink to="/simpsons">Exit</RouterLink>
    	 </Button>
         </div>
         </div>
        </header>
        
        <main>
         <RouterView />           
        </main>

        <footer class="bg-simpsons-yellow w-full border border-black text-center py-6">
            <div>
                <strong>All Rights Reserved</strong> - Oh Lord Matt Groening - 1989-2026
            </div>

            <small>
                This app was done by Mateo Olascoaga
            </small>

        </footer>
    

    </div>

</template>

<style scoped>

</style>