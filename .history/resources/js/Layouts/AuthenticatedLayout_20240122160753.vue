<script setup>
import { ref } from 'vue';
import { Link } from '@inertiajs/vue3';
import MapMarkerOutlineIcon from 'vue-material-design-icons/MapMarkerOutline.vue';
import MenuDownIcon from 'vue-material-design-icons/MenuDown.vue';


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
                        <div>
                            <div class="text-[13px] text-grey-300 font-extrabold">
                            <div>Delivery to Morne</div>
                            </div>
                            <div class="text-[15px] text-white -mt-1.5 font-extrabold">
                                <div>Delivery to Morne</div>
                            </div>
                        </div>
                    </div>
                </div>
            <div class="flex grow items-center h-[45px]"></div> 
                <div class="flex items-center justify-center bg-gray-100 border-r border-r-gray-300 font-extrabold text-[11px] text-gray-600 w-[60px] h-[40px] rounded-l-md cursor-pointer">
                    <div class="pt-[3px]">
                        All
                    </div>
                    <MenuDownIcon fillColor="#5e5e5e" :size="20" class="mr-2"/>
                </div>   
            </div>
        </div>
    </div>
</template>
