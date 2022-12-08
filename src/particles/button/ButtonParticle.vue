<script setup lang="ts">
    const props = defineProps({
        level:{type:String, required:false, default:"1"},
        color:{type:String, required:false, default:"primary"},
        label:{type:String, required:false, default:"Label"},
    });
</script>

<template>
    <button :class="`f-btn level-${level}-${color}`">
        {{ label }}
    </button>
</template>