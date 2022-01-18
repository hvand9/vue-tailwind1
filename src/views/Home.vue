<!-- This example requires Tailwind CSS v2.0+ -->
<template>



    <section class="bg-black dark:bg-gray-800">
        <nav class="container p-6 mx-auto lg:flex lg:justify-between lg:items-center">
            <div class="flex items-center justify-between">
                <div>
                    <a class="text-2xl font-bold text-gray-800 dark:text-white lg:text-3xl hover:text-gray-700 dark:hover:text-gray-300" href="~@/assets/APEX.jpg"></a>
                    <img class="logo" src="~@/assets/logo.png" width="150" height="200">
                </div>
    
                <!-- Mobile menu button -->
                <div class="flex lg:hidden">
                    <button type="button"
                        class="text-gray-500 hover:text-gray-600 focus:outline-none focus:text-gray-600"
                        aria-label="toggle menu">
                        <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
                            <path fill-rule="evenodd"
                                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z">
                            </path>
                        </svg>
                    </button>
                </div>
            </div>

            

            <!--
          {{ todo.text }}
        -->
              <!-- Comment -->
            <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
           <!-- <div class="flex flex-col mt-4 space-y-2 lg:mt-0 lg:flex-row lg:-px-8 lg:space-y-0">
                <a class="mx-8 text-gray-700 transition-colors duration-200 transform dark:text-gray-200 dark:hover:text-blue-400 hover:text-blue-500"
                    href="#">Home</a>
                <a class="mx-8 text-gray-700 transition-colors duration-200 transform dark:text-gray-200 dark:hover:text-blue-400 hover:text-blue-500"
                    href="#">Components</a>
                <a class="mx-8 text-gray-700 transition-colors duration-200 transform dark:text-gray-200 dark:hover:text-blue-400 hover:text-blue-500"
                    href="#">Pricing</a>
                <a class="mx-8 text-gray-700 transition-colors duration-200 transform dark:text-gray-200 dark:hover:text-blue-400 hover:text-blue-500"
                    href="#">Contact</a>
            </div> -->
    
            <a class="block px-5 py-2 mt-4 font-medium leading-5 text-center text-white capitalize bg-blue-600 rounded-lg lg:mt-0 hover:bg-blue-500 lg:w-auto"
                href="#">
                Se stats
            </a>
        </nav>
    
        <div class="container px-6 py-16 mx-auto text-center">
            <div class="max-w-lg mx-auto">
                <h1 class="text-3xl font-bold text-gray-800 dark:text-white md:text-4xl">Gamingstats</h1>
                <p class="mt-6 text-gray-500 dark:text-gray-300">Her kan du se alle dine venners gamingstats inden du joiner dem. Se alt fra kills og wins</p>
                <button
                    class="px-6 py-2 mt-6 text-sm font-medium leading-5 text-center text-white capitalize bg-blue-600 rounded-lg hover:bg-blue-500 md:mx-0 md:w-auto focus:outline-none">
    <router-link class="font-semibold text-gray-700 hover:underline" to="/hello">Se stats</router-link>
                </button>
            </div>

            
    
            <div class="flex justify-center mt-10">
                <div class="w-full h-30 bg-black-200 rounded-xl md:w-4/5">
                <br>
                <br>



      
    <div class="max-w-xs mx-auto overflow-hidden bg-white rounded-lg shadow-lg dark:bg-gray-800">
        <div class="px-2 py-2">
            <h1 class="text-3xl font-bold text-gray-800 uppercase dark:text-white">Apex Legends</h1>
            <p class="mt-1 text-sm text-gray-600 dark:text-gray-400">Apex Legends er et af de mest populære spil blandt vores spiller. Her kan du se dine venners stats inden du tilslutter dig til dem.</p>
        </div>

        <img class="object-cover w-full h-48 mt-2" src="~@/assets/APEX.jpg" alt="NIKE AIR">

        <div class="flex items-center justify-between px-4 py-2 bg-gray-900">
            <h1 class="text-lg font-bold text-white">Battle Royale</h1>
                <router-link class="px-2 py-1 text-xs font-semibold text-gray-900 uppercase transition-colors duration-200 transform bg-white rounded hover:bg-gray-200 focus:bg-gray-400 focus:outline-none" to="/apex">Se stats</router-link>
        </div>
    </div>

    <br>
    <br>

    
    <div class="max-w-xs mx-auto overflow-hidden bg-white rounded-lg shadow-lg dark:bg-gray-800">
        <div class="px-4 py-2">
            <h1 class="text-3xl font-bold text-gray-800 uppercase dark:text-white">Counter Strike</h1>
            <p class="mt-1 text-sm text-gray-600 dark:text-gray-400">Counter Strike er et af de mest populære spil blandt vores spiller. Her kan du se dine venners stats inden du tilslutter dig til dem.</p>
        </div>

        <img class="object-cover w-full h-48 mt-2" src="~@/assets/CSGO.jpg" alt="NIKE AIR">

        <div class="flex items-center justify-between px-4 py-2 bg-gray-900">
            <h1 class="text-lg font-bold text-white">CS GO</h1>
                <router-link class="px-2 py-1 text-xs font-semibold text-gray-900 uppercase transition-colors duration-200 transform bg-white rounded hover:bg-gray-200 focus:bg-gray-400 focus:outline-none" to="/csgo">Se stats</router-link>
        </div>
    </div>

    <br>
    <br>

     <div class="max-w-xs mx-auto overflow-hidden bg-white rounded-lg shadow-lg dark:bg-purple-800">
        <div class="px-4 py-2">
            <h1 class="text-3xl font-bold text-gray-800 uppercase dark:text-white">Call Of Duty</h1>
            <p class="mt-1 text-sm text-gray-600 dark:text-gray-400">Call Of Duty er et af de mest populære spil blandt vores spiller. Her kan du se dine venners stats inden du tilslutter dig til dem.</p>
        </div>

        <img class="object-cover w-full h-48 mt-2" src="~@/assets/WARZONE.jpg" alt="NIKE AIR">

        <div class="flex items-center justify-between px-4 py-2 bg-gray-900">
            <h1 class="text-lg font-bold text-white">Warzone</h1>
                <router-link class="px-2 py-1 text-xs font-semibold text-gray-900 uppercase transition-colors duration-200 transform bg-white rounded hover:bg-gray-200 focus:bg-gray-400 focus:outline-none" to="/hello">Se stats</router-link>
        </div>
    </div>

    <br>
    <br>
    
              
                </div>
            </div>
        </div>
        


  <div class="max-w-screen-xl mx-auto mt-10">
                <div class="grid grid-cols-2 gap-8 md:grid-cols-6 lg:grid-cols-5">
                    <div class="flex items-center justify-center col-span-1 md:col-span-2 lg:col-span-1">
                    <img class="logo" src="~@/assets/csgo1.png" width="100" height="100">
                    </div>

                    <div class="flex items-center justify-center col-span-1 md:col-span-2 lg:col-span-1">
                    <img class="logo" src="~@/assets/fortnite.png" width="60" height="60">
                    </div>

                    <div class="flex items-center justify-center col-span-1 md:col-span-2 lg:col-span-1">
                    <img class="logo" src="~@/assets/gta2.png" width="60" height="60">
                    </div>

                    <div class="flex items-center justify-center col-span-1 md:col-span-3 lg:col-span-1">
                    <img class="logo" src="~@/assets/apex2.png" width="60" height="60">
                    </div>
                    
                    <div class="flex items-center justify-center col-span-2 md:col-span-3 lg:col-span-1">
                    <img class="logo" src="~@/assets/logo.png" width="60" height="60">
                    </div>
                </div>
            </div>

        
    </section>

    

  
</template>

