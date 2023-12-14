<script setup>
    import SidebarTitle from "@/components/SidebarTitle.vue";
</script>

<template>
    <div class="flex flex-col justify-between">
        <div>
            <SidebarTitle title="TO-DO"></SidebarTitle>
            <div class="ml-3 p-3 space-y-3 overflow-y-auto text-gray-800 max-h-[calc(100vh-10rem)]">
                <label class="inline-block"><input type="checkbox" name="" id="" /> Making a Vue project </label>
                <label class="inline-block line-through"><input type="checkbox" checked name="" id="" /> Doing something else </label>
            </div>
        </div>
        <button class="px-10 py-2 bg-red-100 w-fit mx-auto my-5 hover:bg-red-200 shadow-md">ADD NEW</button>
    </div>
</template>
