<script setup>
    import ToDoList from "@/components/ToDoList";
    import MainTitle from "@/components/MainTitle";
    import MainTimer from "@/components/MainTimer";
    import InspirationalQuote from "@/components/InspirationalQuote";
    import TimeLog from "@/components/TimeLog";
</script>

<template>
    <div class="py-10 grid grid-cols-4 gap-20 text-red-400 bg-red-50 h-screen">
        <ToDoList class="border border-red-200 bg-white" />
        <div class="flex flex-col justify-between border col-span-2 text-center py-10">
            <div class="h-2/3 my-auto">
                <MainTitle title="Time to work!" />
                <MainTimer />

                <button class="px-10 py-2 bg-red-100 w-fit mx-auto my-3 hover:bg-red-200 shadow-md">START</button>
            </div>
            <!-- <Suspense> -->
            <!-- <template #default> -->
            <InspirationalQuote />
            <!-- </template>
                <template #fallback>
                    <span>Loading...</span>
                </template> -->
            <!-- </Suspense> -->
        </div>
        <TimeLog class="border border-red-200 bg-white" />
    </div>
</template>

<style>
    #app {
        font-family: Arial, sans-serif;
    }
</style>
