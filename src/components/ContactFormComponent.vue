<script setup> </script>
<template>
    <form class="ml-auo space-y-4">
        <input type='text' placeholder='Votre nom'
            class="w-full rounded-md py-3 px-4 bg-gray-100 text-sm outline-amber-200" />
        <input type='email' placeholder='Votre adresse email'
            class="w-full rounded-md py-3 px-4 bg-gray-100 text-sm outline-amber-200" />
        <input type='tel' placeholder='Votre numéro de téléphone'
            class="w-full rounded-md py-3 px-4 bg-gray-100 text-sm outline-amber-200" />
        <textarea placeholder='Votre message' rows="6"
            class="w-full rounded-md px-4 bg-gray-100 text-sm pt-3 outline-amber-200"></textarea>
        <div class="flex justify-center">
            <button type='button'
            class="bg-secondary text-white font-bold rounded-md text-sm px-4 py-3 w-1/3">Prendre contact</button>
        </div>
    </form>
</template>

<style scoped>
</style>