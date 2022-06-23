<template>
    <h1 class="text-white text-xl text-center pt-12">{{ msg }}</h1>
    <div class="text-center mt-8">
        <button class="bg-transparent border border-white px-4 py-2 rounded-2xl text-white font-normal" @click="action">click me</button>
    </div>
</template>

<script setup>
    defineProps({
        msg: String
    })

    const action = () => {
        window.alert('clicked')
    }
</script>