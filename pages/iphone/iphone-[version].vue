<template>
        <div class="flex justify-center text-2xl">
            <p>IPhone - {{ iphoneVersion }}</p>
        </div>
</template>

<script setup>
 const route = useRoute()

 const iphoneVersion = computed(() => {
    return route.params.version.replaceAll('-', ' ');
 })

</script>
