<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
import Welcome from '@/Jetstream/Welcome.vue';
import { Word } from '@/Pages/components/Word.vue';
</script>

<template>
    <AppLayout title="Dashboard">
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                에어컨
            </h2>

        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                <div class="bg-white overflow-hidden shadow-xl sm:rounded-lg">
                    <Word pr={{k}}/>
                </div>
            </div>
        </div>
    </AppLayout>
</template>
<script>
export default {
    data() {
        return {
            k: {
                a:"1",
                b:"2"
            }
        }
    }
}
</script>
