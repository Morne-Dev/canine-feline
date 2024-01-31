<script setup>
import { ref } from 'vue';
import { Link } from '@inertiajs/vue3';
import MapMarkerOutlineIcon from 'vue-material-design-icons/MapMarkerOutline.vue';

const showingNavigationDropdown = ref(false);
</script>

<template>
    <div class="min-w-[1150px] bg-gray-100 h-full">
        <div class="flex items-center bg-gray-900 h-[60px] py-2 fixed z-50 min-w-[1150px] w-full">
            <div class="flex">
                <Link class=" text-white h-[50] p-2 pt-3 border-[1px] border-grey-900 rounded-sm hover:border-[1px] hover:border-gray-100 cursor-pointer">
                    Canine & Feline
                </Link>
                <div class=" text-white h-[50] p-2 pt-3 border-[1px] border-grey-900 rounded-sm hover:border-[1px] hover:border-gray-100 cursor-pointer">
                    <div class="flex items-center justify-center">
                        <MapMarkerOutlineIcon class="pt-2 -ml-1"  fillColor="#f5f5f5"/>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
