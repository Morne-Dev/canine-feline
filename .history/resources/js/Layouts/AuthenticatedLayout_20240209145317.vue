<script setup>
import { ref } from 'vue';
import { Link } from '@inertiajs/vue3';
import MapMarkerOutlineIcon from 'vue-material-design-icons/MapMarkerOutline.vue';
import MenuDownIcon from 'vue-material-design-icons/MenuDown.vue';
import MagnifyIcon from 'vue-material-design-icons/Magnify.vue';
import CartMinusIcon from 'vue-material-design-icons/CartMinus.vue';
import MenuIcon from 'vue-material-design-icons/Menu.vue';

const showingNavigationDropdown = ref(false);
</script>

<template>
    <div class="min-w-[1150px] bg-gray-100 h-full">
        <div class="flex items-center bg-gray-900 h-[70px] py-2 fixed z-50 min-w-[1150px] w-full">
            <div class="flex">
                <Link href="/your-desired-path" class="text-white h-[50] p-2 pt-3 border-[1px] border-transparent rounded-sm hover:border-gray-100 cursor-pointer">
                    Canine & Feline
                </Link>
            </div>
            <div class="text-white h-[50] p-2 border-[1px] border-transparent rounded-sm hover:border-gray-100 cursor-pointer">
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
            <div class="flex grow items-center h-[45px] px-1">
                <div class="flex items-center justify-center bg-gray-100 border-r border-r-gray-300 font-extrabold text-[11px] text-grey-600 w-[60px] h-[40px] rounded-l-md cursor-pointer">
                    <div class="pt-[3px]">
                        All
                    </div>
                    <menuDownIcon fillColor="#5e5e5e" :size="20" class="-mr-2"/>
                </div>
                <input class="block w-full border-none border-transparent focus:border-transparent focus:ring-0" type="text"/>
                <div class="cursor-pointer bg-orange-300 p-[5px] px-2 rounded-r-md">
                    <MagnifyIcon :size="30"/>
                </div>
            </div>
            <div class="flex">
                <div class="h-[50px] p-2 border-[1px] border-transparent rounded-sm hover:border-gray-100 cursor-pointer">
                    <div class="flex items-center justify-center mt-2.5 px-1">
                        <img src="https://via.placeholder.com/35x20" alt=""/>
                        <div class="text-[15px] text-white -mt-2 -mr-0.5 font-extrabold">EN</div>
                        <menuDownIcon fillColor="#c2c2c2" :size="20" class="-mr-2 -mt-1.5"/>
                    </div>
                </div>

                <div class="h-[50px] p-2 border-[1px] border-transparent rounded-sm hover:border-gray-100 cursor-pointer">
                    <div class="flex items-center justify-center">
                        <div>
                            <div class="text-[12px] text-white font-extrabold">
                                Hello,
                                <span>Sign In</span>
                            </div>
                            <div class="flex items-center">
                                <div class="text-[15px] text-white -mt-1.5 font-extrabold">Account and List</div>
                                <menuDownIcon fillColor="#c2c2c2" :size="20" class="-mr-2 -mt-1.5"/>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="h-[50px] p-2 border-[1px] border-transparent rounded-sm hover:border-gray-100 cursor-pointer">
                    <div class="flex items-center justify-center">
                        <div>
                            <div class="text-[12px] text-white font-extrabold">
                                Returns,
                            </div>
                            <div class="flex items-center">
                                <div class="text-[15px] text-white -mt-1.5 font-extrabold">& Orders</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="relative h-[50px] p-2 border-[1px] border-transparent rounded-sm hover:border-gray-100 cursor-pointer">
                    <span class="absolute text-center right-[21px] w-14px -top-0 rounded-full text-[20px]">
                        <div class="text-orange-400 font-extrabold bg-gray-900 h-[16px]">0</div>
                    </span>
                    <div class="flex items-center justify-center">
                        <CartMinusIcon fillColor="#fcfcfc" :size="40" class="-mt-0.5"/>
                    </div>
                </div>
            </div>
        </div>
        <div class="flex items-center justify-between bg-[#232f3e] h-[38px] fixed z-40 min-w-[1150px] w-full mt-[60px]">
            <div class="flex">
                <div class="flex h-[30px] border-[1px] bg-[#232f3e] rounded-sm hover:border-[1px] hover:border-gray-100 cursor-pointer">
                    <div class="flex items-center justify-between px-2">
                        <MenuIcon fillColor="#F5F5F5" size="26" class="mr-0.5" />
                        <div class="text-[14px]" text-white font-extrabold>All</div>
                    </div>
                </div>
                <div class="flex h-[30px] border-[1px] bg-[#232f3e] rounded-sm hover:border-[1px] hover:border-gray-100 cursor-pointer">
                    <div class="flex items-center justify-between px-2">
                        <div class="text-[14px]" text-white font-extrabold>Today's Deals</div>
                    </div>
                </div>
            </div>
        </div>

        <main class="max-w-[1500px] mx-auto">
            <div class="pt-[98px]"></div>
            <slot></slot>
        </main>

        <div class="w-full bg-white mt-10">
            <div class="max-w-[1500px] mx-auto">
                <div class="text-[23px] pt-4 font-extrabold">Recommended based on your shopping trends</div>
                <div class="flex justify-center items-stretch">
                    <div class="p-4 text-center mx-auto">
                        <div class="w-[158px] h-[150px] overflow-hidden">
                            <img src="https://via.placeholder.com/158x150" alt="">
                        </div>
                        <div class="w-[160px] text-[12px] py-2 text-teal-600 font-extrabold hover:text-red-600 cursor-pointer">
                            This is a test Title
                        </div>
                        <div class="flex justify-start">
                            <div class="text-xs font-extrabold text-red-600 w-full text-left">$99.99</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <footer class="bg-[#232F3E]">
            <div class="bg-[#37475A] hover:bg-gray-600 w-full p-3.5 cursor-pointer text-white font-extrabold text-center">
                Back to top
            </div>
            <div class="flex items-stretch justify-between max-w-[1000px] mx-auto p-10 text-white">
                <ul>
                    <li class=" font-extrabold text-lg">Get to Know Us</li>
                    <li class="hover:underline cursor-pointer">Careers</li>
                    <li class="hover:underline cursor-pointer">About Canine & Feline</li>
                    <li class="hover:underline cursor-pointer">Investor Relations</li>
                    <li class="hover:underline cursor-pointer">Canine & Feline Devices</li>
                    <li class="hover:underline cursor-pointer">Canine & Feline Science</li>

                </ul>

                <ul>
                    <li class=" font-extrabold text-lg">Make Money with US</li>
                    <li class="hover:underline cursor-pointer">Sell products on Amazon</li>
                    <li class="hover:underline cursor-pointer">Sell on Amazon</li>
                    <li class="hover:underline cursor-pointer">Sell apps on Amazon</li>
                    <li class="hover:underline cursor-pointer">Become an Affiliate</li>
                    <li class="hover:underline cursor-pointer">Advertise Your Products</li>
                    <li class="hover:underline cursor-pointer">Self-Publish with Us</li>
                    <li class="hover:underline cursor-pointer">Host on Amazon Hub</li>

                </ul>

                <ul>
                    <li class=" font-extrabold text-lg">Get to Know Us</li>
                    <li class="hover:underline cursor-pointer">Careers</li>
                    <li class="hover:underline cursor-pointer">About Canine & Feline</li>
                    <li class="hover:underline cursor-pointer">Investor Relations</li>
                    <li class="hover:underline cursor-pointer">Canine & Feline Devices</li>
                    <li class="hover:underline cursor-pointer">Canine & Feline Science</li>

                </ul>

                <ul>
                    <li class=" font-extrabold text-lg">Make Money with US</li>
                    <li class="hover:underline cursor-pointer">Sell products on Amazon</li>
                    <li class="hover:underline cursor-pointer">Sell on Amazon</li>
                    <li class="hover:underline cursor-pointer">Sell apps on Amazon</li>
                    <li class="hover:underline cursor-pointer">Become an Affiliate</li>
                    <li class="hover:underline cursor-pointer">Advertise Your Products</li>
                    <li class="hover:underline cursor-pointer">Self-Publish with Us</li>
                    <li class="hover:underline cursor-pointer">Host on Amazon Hub</li>

                </ul>
            </div>
        </footer>
    </div>
</template>
