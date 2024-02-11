<script>
    import { Link } from "svelte-navigator";

</script>
<!-- <nav class="navbar bg-base-100 sm:items-start">
    <div class="justify-around w-1/2">
        <div class="relative">
            <img
                loading="lazy"
                src="AR-logo.svg"
                alt=""
                class="aspect-square object-contain object-center w-20 sm:w-28 overflow-hidden shrink-0 max-w-full"
            />
        </div>
    </div>
    <div class="navbar-center hidden lg:flex">
        <ul class="menu menu-horizontal px-1 gap-12">
            <a class="text-slate-700 text-xl font-medium leading-6 whitespace-nowrap" href="/">Home</a>
            <a class="text-slate-700 text-xl font-medium leading-6 whitespace-nowrap" href="#about">About</a>
            <a class="text-slate-700 text-xl font-medium leading-6 whitespace-nowrap" href="#services">Services</a>
            <a class="text-slate-700 text-xl font-medium leading-6 whitespace-nowrap" href="#testimonials">Newsletter</a>
        </ul>
    </div>
    <div class="navbar-end md:justify-evenly">
        <a class="hidden sm:inline-flex btn bg-blue-600 hover:bg-blue-500 rounded-lg text-white" href="/">Connect</a
        >
        <div class="dropdown">
            <div tabindex="0" role="button" class="btn btn-ghost md:hidden">
                <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-5 w-5 rotate-180"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                    ><path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M4 6h16M4 12h8m-8 6h16"
                    /></svg
                >
            </div>
            <ul
                class="menu menu-sm dropdown-content mt-3 z-[1] p-4 shadow bg-white rounded-box w-60"
            >
            <a class="font-medium leading-6 whitespace-nowrap" href="/">Home</a>
            <a class="font-medium leading-6 whitespace-nowrap" href="#about">About</a>
            <a class="font-medium leading-6 whitespace-nowrap" href="#services">Services</a>
            <a class="font-medium leading-6 whitespace-nowrap" href="#testimonials">Testimonials</a>
            </ul>
        </div>
    </div>
    
</nav> -->
<nav class="z-10 w-full bg-white dark:bg-transparent md:bg-transparent">
    <div class="container m-auto px-2 md:px-12 lg:px-7">
        <div class="flex flex-wrap items-center justify-between py-3 gap-6 md:py-4 md:gap-0">
            <input type="checkbox" name="toggle_nav" id="toggle_nav" class="peer hidden">
            <div class="w-full px-6 flex justify-between lg:w-max md:px-0 z-30">
                <a href="/" aria-label="logo" class="flex space-x-2 items-center">
                    <img src="/AR-logo.svg" class="w-[4.5rem] lg:w-28" alt="AR logo">
                    <!-- <span class="text-2xl font-bold text-blue-900 dark:text-white">AR Business <span class="text-blue-700 dark:text-blue-300"> Consultant</span></span> -->
                </a>

                <div class="flex items-center lg:hidden max-h-10">
                    <label role="" for="toggle_nav" aria-label="humburger" id="hamburger" class="relative w-10 h-auto p-2">
                        <div id="line"
                            class="m-auto h-0.5 w-6 rounded bg-blue-900 dark:bg-white transition duration-300"></div>
                        <div id="line2"
                            class="m-auto mt-2 h-0.5 w-6 rounded bg-blue-900 dark:bg-white transition duration-300">
                        </div>
                    </label>
                </div>
            </div>

            <label role="" for="toggle_nav" class="hidden peer-checked:block fixed w-full h-full left-0 top-0 z-10 bg-blue-200 dark:bg-black dark:bg-opacity-80 bg-opacity-30 backdrop-blur backdrop-filter"></label>
            <div class="hidden peer-checked:flex w-full flex-col lg:flex lg:flex-row justify-end z-30 items-center gap-y-6 p-6 rounded-xl bg-white dark:bg-gray-900 lg:gap-y-0 lg:p-0 md:flex-nowrap lg:bg-transparent lg:w-7/12">
                <div class="text-gray-600 lg:pr-4 w-full">
                    <ul class="tracking-wide font-medium  text-sm 
                    flex flex-col gap-y-6 lg:gap-y-0 lg:flex-row w-full">
                        <Link to="/">
                            <span class="block md:px-4 transition dark:text-gray-300 dark:hover:text-blue-300 hover:text-blue-700">
                                <span>Home</span>
                            </span>
                        </Link>
                        <Link to="/#about">
                            <div class="block md:px-4 transition dark:text-gray-300 dark:hover:text-blue-300 hover:text-blue-700">
                                <span>About us</span>
                            </div>
                        </Link>
                        <Link to="/services">
                            <div class="block md:px-4 transition dark:text-gray-300 dark:hover:text-blue-300 hover:text-blue-700">
                                <span>Services</span>
                            </div>
                        </Link>
                    </ul>
                </div>

                <div class="w-full min-w-max space-y-2 
                border-blue-200 lg:space-y-0 sm:w-max l:border-l dark:lg:border-gray-700">
                    <!-- <button type="button" title="Start buying" class="w-full py-3 px-6 text-center rounded-full transition active:bg-blue-200 dark:active:bg-gray-700 dark:focus:bg-gray-800 focus:bg-blue-100 sm:w-max">
                        <span class="block text-blue-800 dark:text-white font-semibold text-sm">
                            Sign up
                        </span>
                    </button> -->
                    <Link to="/connect">
                    <button type="button" title="Start buying" class="w-full py-3 px-6 text-center rounded-full transition bg-blue-600 hover:bg-blue-700 active:bg-blue-700 focus:bg-blue-600 sm:w-max">
                        <span  class="block text-white font-semibold text-sm">
                            Connect
                        </span>
                    </button></Link>
                </div>
            </div>
        </div>
    </div>
</nav>