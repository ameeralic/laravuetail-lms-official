<template>
    <section>
        <div class="py-5 px-4 text-center">
            <a :href="whatsNewLink" target="_blank"
                class="inline-flex justify-between items-center py-1 px-1 pr-4 mb-10 text-sm text-gray-300 bg-zinc-800 rounded-full hover:bg-zinc-700"
                role="alert">
                <span class="text-xs bg-vue rounded-full text-white px-4 py-1.5 mr-3">New</span>
                <span class="text-xs font-medium text-left">{{
                    whatsNewText
                }}</span>
                <svg class="ml-2 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd"
                        d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
                        clip-rule="evenodd"></path>
                </svg>
            </a>
            <div class="grid grid-cols-2 place-content-center w-fit mx-auto mb-6 md:mb-10">
                <div class="mr-10">
                    <img :src="$page.props.app_url + 'storage/images/laravuetail-logo.png'" alt=""
                        class="h-10 w-10 md:h-18 md:w-18 mx-auto" />
                    <h1 class="text-sm font-medium tracking-tight leading-none text-gray-400 md:text-sm py-2">
                        <span class="text-[#ff2d20]">Lara</span><span class="text-[#41b883]">Vue</span><span
                            class="text-[#38bdf8]">Tail</span>
                    </h1>
                </div>
                <div class="border-l pl-10">
                    <img :src="$page.props.app_url + 'storage/images/lms-logo.svg'" alt=""
                        class="h-10 w-10 md:h-18 md:w-18 mx-auto" />
                    <h1 class="text-sm tracking-tight leading-none text-gray-200 md:text-sm py-1 font-medium">
                        LVTLearn
                    </h1>
                </div>
            </div>

            <h1
                class=" mb-4 md:mb-8 text-5xl font-bold tracking-tight leading-14 md:leading-7 pb-2 md:py-4 md:text-5xl text-transparent bg-clip-text bg-gradient-to-r from-laravel via-vue to-tailwind">
                {{ projectName }}
            </h1>
            <p class="mb-4 text-sm font-normal text-gray-300 sm:px-16 xl:px-48 dark:text-gray-400">
                {{ projectDescription }}
            </p>
            <div class="grid grid-cols-2 mb-10 w-fit mx-auto place-content-start gap-x-8 gap-y-4 justify-items-start">
                <a href="http://laravel.com" target="_blank" rel="noopener noreferrer"
                    class="flex justify-start text-gray-300 gap-1 text-sm md:text-base items-center w-fit">
                    <img src="https://asset.brandfetch.io/ide68-31CH/idhaVMa0Af.svg" alt="" class="h-4 w-auto" />
                    <p>Laravel</p>
                </a>

                <a href="http://vuejs.com" target="_blank" rel="noopener noreferrer"
                    class="flex justify-start text-gray-300 gap-1 text-sm md:text-base items-center">
                    <img src="https://asset.brandfetch.io/idT-7aLCAj/idYSAxBM8n.svg" alt="" class="h-3 w-auto" />
                    <p>Vue.js</p>
                </a>

                <a href="https://tailwindcss.com
                    " target="_blank" rel="noopener noreferrer"
                    class="flex justify-start text-gray-300 gap-1 text-sm md:text-base items-center">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/d/d5/Tailwind_CSS_Logo.svg" alt=""
                        class="h-4 w-auto" />
                    <p>TailwindCSS</p>
                </a>

                <a href="https://inertiajs.com/" target="_blank" rel="noopener noreferrer"
                    class="flex justify-start text-gray-300 gap-1 text-sm md:text-base items-center">
                    <img src="https://asset.brandfetch.io/idGjvMIqVt/idd9HKmA9r.jpeg" alt="" class="h-4 w-auto" />
                    <p>Inertia.js</p>
                </a>
            </div>
            <div class="flex justify-center mb-8 lg:mb-16 gap-4">
                <Link href="/docs"
                    class="inline-flex cursor-pointer shadow-xl shadow-[#41b883]/40 hover:shadow-[#38bdf8]/90 justify-center items-center py-3 px-4 text-sm font-medium text-center text-white rounded-xl bg-vue hover:bg-tailwind focus:ring-4 focus:ring-primary-300">
                Visit Docs
                <svg class="ml-2 -mr-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd"
                        d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                        clip-rule="evenodd"></path>
                </svg>
                </Link>
                <a :href="projectGitRepoLink" target="_blank"
                    class="inline-flex cursor-pointer shadow-xl hover:shadow-[#38bdf8]/90 shadow-gray-100/50 justify-center items-center py-3 px-4 text-sm font-medium text-center text-gray-800 rounded-xl bg-white hover:bg-tailwind focus:ring-4 focus:ring-primary-300">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 496 512" class="w-5 h-5 mr-3 text-gray-300">
                        <!--! Font Awesome Pro 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
                        <path
                            d="M165.9 397.4c0 2-2.3 3.6-5.2 3.6-3.3.3-5.6-1.3-5.6-3.6 0-2 2.3-3.6 5.2-3.6 3-.3 5.6 1.3 5.6 3.6zm-31.1-4.5c-.7 2 1.3 4.3 4.3 4.9 2.6 1 5.6 0 6.2-2s-1.3-4.3-4.3-5.2c-2.6-.7-5.5.3-6.2 2.3zm44.2-1.7c-2.9.7-4.9 2.6-4.6 4.9.3 2 2.9 3.3 5.9 2.6 2.9-.7 4.9-2.6 4.6-4.6-.3-1.9-3-3.2-5.9-2.9zM244.8 8C106.1 8 0 113.3 0 252c0 110.9 69.8 205.8 169.5 239.2 12.8 2.3 17.3-5.6 17.3-12.1 0-6.2-.3-40.4-.3-61.4 0 0-70 15-84.7-29.8 0 0-11.4-29.1-27.8-36.6 0 0-22.9-15.7 1.6-15.4 0 0 24.9 2 38.6 25.8 21.9 38.6 58.6 27.5 72.9 20.9 2.3-16 8.8-27.1 16-33.7-55.9-6.2-112.3-14.3-112.3-110.5 0-27.5 7.6-41.3 23.6-58.9-2.6-6.5-11.1-33.3 2.6-67.9 20.9-6.5 69 27 69 27 20-5.6 41.5-8.5 62.8-8.5s42.8 2.9 62.8 8.5c0 0 48.1-33.6 69-27 13.7 34.7 5.2 61.4 2.6 67.9 16 17.7 25.8 31.5 25.8 58.9 0 96.5-58.9 104.2-114.8 110.5 9.2 7.9 17 22.9 17 46.4 0 33.7-.3 75.4-.3 83.6 0 6.5 4.6 14.4 17.3 12.1C428.2 457.8 496 362.9 496 252 496 113.3 383.5 8 244.8 8zM97.2 352.9c-1.3 1-1 3.3.7 5.2 1.6 1.6 3.9 2.3 5.2 1 1.3-1 1-3.3-.7-5.2-1.6-1.6-3.9-2.3-5.2-1zm-10.8-8.1c-.7 1.3.3 2.9 2.3 3.9 1.6 1 3.6.7 4.3-.7.7-1.3-.3-2.9-2.3-3.9-2-.6-3.6-.3-4.3.7zm32.4 35.6c-1.6 1.3-1 4.3 1.3 6.2 2.3 2.3 5.2 2.6 6.5 1 1.3-1.3.7-4.3-1.3-6.2-2.2-2.3-5.2-2.6-6.5-1zm-11.4-14.7c-1.6 1-1.6 3.6 0 5.9 1.6 2.3 4.3 3.3 5.6 2.3 1.6-1.3 1.6-3.9 0-6.2-1.4-2.3-4-3.3-5.6-2z" />
                    </svg>
                    <p class="">Github Repo</p>
                </a>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    props: [
        "whatsNewText",
        "whatsNewLink",
        "projectName",
        "projectDescription",
        "projectStack",
        "projectDocsLink",
        "projectGitRepoLink",
    ],
    data() {
        return {};
    },
};
</script>
