<script setup>
import { Head, Link } from '@inertiajs/inertia-vue3';

defineProps({
    canLogin: Boolean,
    canRegister: Boolean,
    laravelVersion: String,
    phpVersion: String,
});
</script>

<template>
    <Head title="Welcome" />

    <div class="relative flex items-top justify-center min-h-screen bg-gray-100 dark:bg-gray-900 sm:items-center sm:pt-0">
        <div v-if="canLogin" class="hidden fixed top-0 right-0 px-6 py-4 sm:block">
            <Link v-if="$page.props.user" :href="route('dashboard')" class="text-sm text-gray-700 dark:text-gray-500 underline">Dashboard</Link>

            <template v-else>
                <Link :href="route('login')" class="text-sm text-gray-700 dark:text-gray-500 underline">Zaloguj się</Link>

                <Link v-if="canRegister" :href="route('register')" class="ml-4 text-sm text-gray-700 dark:text-gray-500 underline">Rejestracja</Link>
            </template>
        </div>

        <div class="max-w-6xl mx-auto sm:px-6 lg:px-8">
            <div class="mt-8 bg-white dark:bg-gray-800 overflow-hidden shadow sm:rounded-lg">
                <div class="grid grid-cols-1 md:grid-cols-2">
                    <div class="p-6">
                        <div class="flex items-center">
                            <svg
                                fill="none"
                                stroke="currentColor"
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                stroke-width="2"
                                viewBox="0 0 24 24"
                                class="w-8 h-8 text-gray-500"
                            ><path d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253" /></svg>
                            <div class="ml-4 text-lg leading-7 font-semibold text-gray-900 dark:text-white">
                                Lorem Ipsum
                            </div>
                        </div>

                        <div class="ml-12">
                            <div class="mt-2 text-gray-600 dark:text-gray-400 text-sm">
                                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis porta mi augue, at semper nisl venenatis vitae. Vivamus dictum lorem non ex rutrum, vitae condimentum odio volutpat. Mauris placerat erat sit amet odio pulvinar laoreet. Cras malesuada facilisis fermentum. Pellentesque tincidunt malesuada dolor, eu mattis mi vestibulum at. Etiam in ante sed nisl feugiat malesuada. Duis massa elit, tincidunt ut ultrices sit amet, tristique non leo. In euismod ullamcorper sapien, tincidunt aliquam sapien pellentesque sit amet. Nullam at scelerisque eros. Curabitur eu elit quis nisi pharetra pretium ac vitae orci. Aenean sodales tortor nec mauris feugiat dapibus. Sed at arcu velit. Cras magna leo, tempor a maximus sed, fringilla nec dolor.
                            </div>
                        </div>
                    </div>

                    <div class="p-6 border-t border-gray-200 dark:border-gray-700 md:border-t-0 md:border-l">
                        <div class="flex items-center">
                            <svg
                                fill="none"
                                stroke="currentColor"
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                stroke-width="2"
                                viewBox="0 0 24 24"
                                class="w-8 h-8 text-gray-500"
                            ><path d="M3 9a2 2 0 012-2h.93a2 2 0 001.664-.89l.812-1.22A2 2 0 0110.07 4h3.86a2 2 0 011.664.89l.812 1.22A2 2 0 0018.07 7H19a2 2 0 012 2v9a2 2 0 01-2 2H5a2 2 0 01-2-2V9z" /><path d="M15 13a3 3 0 11-6 0 3 3 0 016 0z" /></svg>
                            <div class="ml-4 text-lg leading-7 font-semibold text-gray-900 dark:text-white">
                                Lorem Ipsum
                            </div>
                        </div>

                        <div class="ml-12">
                            <div class="mt-2 text-gray-600 dark:text-gray-400 text-sm">
                                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis porta mi augue, at semper nisl venenatis vitae. Vivamus dictum lorem non ex rutrum, vitae condimentum odio volutpat. Mauris placerat erat sit amet odio pulvinar laoreet. Cras malesuada facilisis fermentum. Pellentesque tincidunt malesuada dolor, eu mattis mi vestibulum at. Etiam in ante sed nisl feugiat malesuada. Duis massa elit, tincidunt ut ultrices sit amet, tristique non leo. In euismod ullamcorper sapien, tincidunt aliquam sapien pellentesque sit amet. Nullam at scelerisque eros. Curabitur eu elit quis nisi pharetra pretium ac vitae orci. Aenean sodales tortor nec mauris feugiat dapibus. Sed at arcu velit. Cras magna leo, tempor a maximus sed, fringilla nec dolor.
                            </div>
                        </div>
                    </div>

                    <div class="p-6 border-t border-gray-200 dark:border-gray-700">
                        <div class="flex items-center">
                            <svg
                                fill="none"
                                stroke="currentColor"
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                stroke-width="2"
                                viewBox="0 0 24 24"
                                class="w-8 h-8 text-gray-500"
                            ><path d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z" /></svg>
                            <div class="ml-4 text-lg leading-7 font-semibold text-gray-900 dark:text-white">
                                Lorem Ipsum
                            </div>
                        </div>

                        <div class="ml-12">
                            <div class="mt-2 text-gray-600 dark:text-gray-400 text-sm">
                                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis porta mi augue, at semper nisl venenatis vitae. Vivamus dictum lorem non ex rutrum, vitae condimentum odio volutpat. Mauris placerat erat sit amet odio pulvinar laoreet. Cras malesuada facilisis fermentum. Pellentesque tincidunt malesuada dolor, eu mattis mi vestibulum at. Etiam in ante sed nisl feugiat malesuada. Duis massa elit, tincidunt ut ultrices sit amet, tristique non leo. In euismod ullamcorper sapien, tincidunt aliquam sapien pellentesque sit amet. Nullam at scelerisque eros. Curabitur eu elit quis nisi pharetra pretium ac vitae orci. Aenean sodales tortor nec mauris feugiat dapibus. Sed at arcu velit. Cras magna leo, tempor a maximus sed, fringilla nec dolor.
                            </div>
                        </div>
                    </div>

                    <div class="p-6 border-t border-gray-200 dark:border-gray-700 md:border-l">
                        <div class="flex items-center">
                            <svg
                                fill="none"
                                stroke="currentColor"
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                stroke-width="2"
                                viewBox="0 0 24 24"
                                class="w-8 h-8 text-gray-500"
                            ><path d="M3.055 11H5a2 2 0 012 2v1a2 2 0 002 2 2 2 0 012 2v2.945M8 3.935V5.5A2.5 2.5 0 0010.5 8h.5a2 2 0 012 2 2 2 0 104 0 2 2 0 012-2h1.064M15 20.488V18a2 2 0 012-2h3.064M21 12a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                            <div class="ml-4 text-lg leading-7 font-semibold text-gray-900 dark:text-white">
                                Lorem Ipsum
                            </div>
                        </div>

                        <div class="ml-12">
                            <div class="mt-2 text-gray-600 dark:text-gray-400 text-sm">
                                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis porta mi augue, at semper nisl venenatis vitae. Vivamus dictum lorem non ex rutrum, vitae condimentum odio volutpat. Mauris placerat erat sit amet odio pulvinar laoreet. Cras malesuada facilisis fermentum. Pellentesque tincidunt malesuada dolor, eu mattis mi vestibulum at. Etiam in ante sed nisl feugiat malesuada. Duis massa elit, tincidunt ut ultrices sit amet, tristique non leo. In euismod ullamcorper sapien, tincidunt aliquam sapien pellentesque sit amet. Nullam at scelerisque eros. Curabitur eu elit quis nisi pharetra pretium ac vitae orci. Aenean sodales tortor nec mauris feugiat dapibus. Sed at arcu velit. Cras magna leo, tempor a maximus sed, fringilla nec dolor.
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="flex justify-center mt-4 sm:items-center sm:justify-between">
                <div class="ml-4 text-center text-sm text-gray-500 sm:text-right sm:ml-0">
                    Laravel v{{ laravelVersion }} (PHP v{{ phpVersion }})
                </div>
            </div>
        </div>
    </div>
</template>
