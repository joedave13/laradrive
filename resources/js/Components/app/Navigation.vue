<template>
    <nav class="min-w-[200px]">
        <div class="h-[80px] px-3 flex items-center gap-3">
            <Link :href="route('dashboard')">
            <ApplicationLogo class="block h-9 w-auto fill-current text-gray-800" />
            </Link>
            LaraDrive
        </div>

        <div class="px-3">
            <CreateNewDropdown />

            <div class="py-3">
                <NavLink href="/">My Files</NavLink>
                <NavLink href="/">Shared With Me</NavLink>
                <NavLink href="/">Shared By Me</NavLink>
                <NavLink href="/">Trash</NavLink>
            </div>
        </div>
    </nav>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';
import ApplicationLogo from '@/Components/ApplicationLogo.vue';
import NavLink from '@/Components/NavLink.vue';
import CreateNewDropdown from './CreateNewDropdown.vue';
</script>