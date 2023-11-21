<template>
    <header class="font-sans antialiased" id="app">
        <div class="flex items-center justify-between flex-wrap bg-grey-dark p-6">
            <div class="flex items-center">
                <img src="../assets/logo.png" alt="" class="h-8 w-8">
                <a href="#" class="no-underline text-white text-bold mt-2">
                    <span class="font-semibold text-xl tracking-tight">
                        Example CSS
                    </span>
                </a>
            </div>
            <div class="block sm:hidden">
                <button @click="toggle" class="flex items-center px-3 py-2 border rounded text-grey-dark-lighter border-grey-dark-light hover:text-white hover:border-white">
                    <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
                </button>
            </div>
            <div :class="open ? 'block': 'hidden'" class="w-full flex-grow sm:flex sm:items-center sm:w-auto">
                <div class="text-sm sm:hidden">
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Home
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        About
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Expertise
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Academia
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Portfolio
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Blog
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Contact
                    </a>
                    <div class="flex">
                        <div>
                            <a href="#" class="no-underline inline-block text-sm px-4 py-2 leading-none border rounded text-white border-white hover:border-transparent hover:text-gray hover:bg-white mt-4 sm:mt-0 mr-2">Register</a>
                        </div>
                        <div>
                            <a href="#" class="no-underline inline-block text-sm px-4 py-2 leading-none border rounded text-white border-white hover:border-transparent hover:text-gray hover:bg-white mt-4 sm:mt-0">Login</a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="hidden w-full block md:flex md:w-auto">
                <div>
                    <a href="#" class="no-underline inline-block text-sm px-4 py-2 leading-none border rounded text-white border-white hover:border-transparent hover:text-gray hover:bg-white mt-4 sm:mt-0 mr-2">Register</a>
                </div>
                <div>
                    <a href="#" class="no-underline inline-block text-sm px-4 py-2 leading-none border rounded text-white border-white hover:border-transparent hover:text-gray hover:bg-white mt-4 sm:mt-0">Login</a>
                </div>
            </div>
        </div>
        <nav class="bg-grey-dark sm:block p-6" :class="open ? 'hidden': 'hidden'">
            <div class="w-full flex-grow sm:flex sm:items-center sm:w-auto">
                <div class="flex justify-center items-center text-sm sm:flex-grow uppercase">
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Home
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        About
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Expertise
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Academia
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Portfolio
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Blog
                    </a>
                    <a href="#" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-white hover:text-white mr-8">
                        Contact
                    </a>
                </div>
            </div>
        </nav>
    </header>
</template>
<script>
    export default  {
        data() {
            return {
                open: false,
            }
        },
        methods: {
            toggle() {
                this.open = !this.open
            }
        }
    }
</script>
<style>

</style>
