<script setup>
import { RouterLink, RouterView } from 'vue-router'
import { HomeIcon } from "@heroicons/vue/20/solid";

</script>

<template>
    <header>

        <div class="container w-full mx-auto">
            <div class="border-b border-gray-200 dark:border-gray-700 ">
                <nav>
                    <ul
                        class="flex flex-wrap -mb-px text-sm font-medium justify-center text-center text-gray-500 dark:text-gray-400">
                        <li class="mr-2">
                            <RouterLink to="/"
                                class="inline-flex p-4 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300 group">
                                <HomeIcon class="w-5 h-5 mr-2 text-gray-600 dark:text-gray-500" />Home
                            </RouterLink>
                        </li>
                        <li class="mr-2">
                            <RouterLink to="/application"
                                class="inline-flex p-4 text-gray-600 rounded-t-lg hover:text-gray-600 dark:text-gray-500 dark:border-gray-500 group">
                                <svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-600 dark:text-gray-500"
                                    fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                                    <path
                                        d="M5 3a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2V5a2 2 0 00-2-2H5zM5 11a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 00-2-2H5zM11 5a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V5zM11 13a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z">
                                    </path>
                                </svg>Application
                            </RouterLink>
                        </li>
                    </ul>
                </nav>
            </div>

        </div>
    </header>

    <RouterView />
</template>

<style scoped>
li a.router-link-exact-active {
    @apply border-gray-600;
    @apply text-gray-600;
    @apply border-b-2;
}

</style>
