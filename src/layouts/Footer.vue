<script setup>
import { useMobileNav } from "@/composables/mobile-nav";

let { loadMobileNav } = useMobileNav();

const year = new Date().getFullYear();
</script>

<template>
    <!-- Footer -->
    <footer :class="loadMobileNav ? 'pb-24 pt-6' : 'py-6'" class="bg-[#0B1120] text-slate-300">
        <p class="text-center text-sm md:text-base">{{ year }} &copy; Criado por <a target="_blank" href="https://github.com/guilasinskas" class="text-secondary-400 font-medium underline underline-offset-4">Guilherme Lasinskas</a></p>
    </footer>
    <!-- Footer -->
</template>
