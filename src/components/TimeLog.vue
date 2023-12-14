<script setup>
    import SidebarTitle from "@/components/SidebarTitle.vue";

    const compliments = ["Great work, dude!", "Keep it up.", "You are on the right path!"];
</script>

<template>
    <div>
        <SidebarTitle title="Time log"></SidebarTitle>

        <div class="relative overflow-y-auto max-h-[calc(100vh-10rem)]">
            <table class="w-full text-sm text-left rtl:text-right text-gray-500 dark:text-gray-400">
                <thead class="text-xs text-gray-700 uppercase bg-gray-50 dark:bg-gray-700 dark:text-gray-400">
                    <tr>
                        <th scope="col" class="px-6 py-3">Time</th>
                        <th scope="col" class="px-6 py-3">Task</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="time-record">
                        <th scope="row">8:30 - 9:10</th>
                        <td>Making a Vue project</td>
                    </tr>
                    <tr class="time-record task-completed">
                        <th scope="row">10:09</th>
                        <td>
                            <span class="italic font-bold text-red-400">Completed task "Doing something else"!</span> <br />
                            <span class="text-black"> {{ compliments[Math.floor(Math.random() * compliments.length)] }}</span>
                        </td>
                    </tr>
                    <tr class="time-record">
                        <th scope="row">9:30 - 10:10</th>
                        <td>Doing something else</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>

<style>
    .time-record {
        background-color: white;
        > * {
            padding: 0.7rem 0.2rem 0.7rem 1.5rem;
        }
        th {
            font-weight: 500;
            white-space: nowrap;
        }
    }
    .task-completed {
        background-color: rgb(254, 226, 226);
        border-top: 1px solid rgb(254, 202, 202);
        border-bottom: 1px solid rgb(254, 202, 202);
        th {
            color: rgb(248, 113, 113);
        }
    }
</style>
