<template>

     <section class="bg-white dark:bg-gray-800">
        <nav class="container p-6 mx-auto lg:flex lg:justify-between lg:items-center">
            <div class="flex items-center justify-between">
                <div>
                    <a class="text-2xl font-bold text-gray-800 dark:text-white lg:text-3xl hover:text-gray-700 dark:hover:text-gray-300" href="#"></a>
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
    
            <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
            <div class="flex flex-col mt-4 space-y-2 lg:mt-0 lg:flex-row lg:-px-8 lg:space-y-0">
                <a class="mx-8 text-gray-700 transition-colors duration-200 transform dark:text-gray-200 dark:hover:text-blue-400 hover:text-blue-500"
                    href="#"><router-link class="font-semibold text-gray-700 hover:underline" to="/">Forside</router-link></a>
            </div>
            

            
    
            <a class="block px-5 py-2 mt-4 font-medium leading-5 text-center text-white capitalize bg-blue-600 rounded-lg lg:mt-0 hover:bg-blue-500 lg:w-auto"
                href="#">
                Se stats
            </a>
        </nav>
    
        <div class="container px-6 py-16 mx-auto text-center">
            <div class="max-w-lg mx-auto">
                <h1 class="text-3xl font-bold text-gray-800 dark:text-white md:text-4xl">Call Of Duty Warzone</h1>
                <p class="mt-6 text-gray-500 dark:text-gray-300">Her kan du se alle stats for Call Of Duty Warzone</p>
                
            </div>

            <img class="object-cover w-full h-48 mt-2" src="~@/assets/WARZONE.jpg" alt="NIKE AIR">

            <div class="flex justify-center mt-10">
                <div class="w-full h-64 bg-blue-600 rounded-xl md:w-4/5"><p>hej{{res.br}}</p></div>
                
            </div>
        </div>
    </section>
</template>



<script>
export default { 
  data() {
    return {
      res: [], // placeholder
    };
},
mounted() {

  fetch("https://call-of-duty-modern-warfare.p.rapidapi.com/warzone/Amartin743/psn", {
	"method": "GET",
	"headers": {
		"x-rapidapi-host": "call-of-duty-modern-warfare.p.rapidapi.com",
		"x-rapidapi-key": "a9814bf04emsh831bd7d8b621711p17fee4jsn496f8c67402d"
	}
})
.then(response => response.json())
.then(response => {
  this.res = response;
	console.log(response.br)
})

.catch(err => {
	console.error(err);
})
}
}
</script>


