<script setup>
import { ref } from 'vue';
import { Link } from '@inertiajs/vue3';
import MapMarkerOutlineIcon from 'vue-material-design-icons/MapMarkerOutline.vue';



const showingNavigationDropdown = ref(false);
</script>

<template>
    <div class="min-w-[1150px] bg-gray-100 h-full">
        <div class="flex items-center bg-gray-900 h-[70px] py-2 fixed z-50 min-w-[1150px] w-full">
            <div class="flex">
                <Link class="text-white h-[50] p-2 pt-3 border-[1px] border-transparent rounded-sm hover:border-gray-100 cursor-pointer">
                    Canine & Feline
                </Link>
            </div>
            <div class="text-white h-[50] p-2 pt-3 border-[1px] border-transparent rounded-sm hover:border-gray-100 cursor-pointer">
                <div class="flex items-center justify-center">
                    <MapMarkerOutlineIcon class="pt-1 -ml-1" fillColor="#f5f5f5"/>
                    <div>
                        <div class="text-[13px] text-gray-300 font-extrabold">
                        <div>
                            Deliver to Morne
                        </div>

                        </div>
                        <div class="text-[15px] text-white font-extrabold">
                            <div>
                                South Africa CPT STR
                            </div>
                        </div>
                    </div>
                </div>

            </div>
            <div calss="flex-grow items-center h-[45px] px-1">
                <div class="flex items-center justify-center bg-gray-100 border-r border-r-gray-300 font-extrabold text-[11px] text-grey-600 w-[60] h-[40px] rounded-l-md cursor-pointer">
                    <div class="pt-[3px]">
                        All
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
