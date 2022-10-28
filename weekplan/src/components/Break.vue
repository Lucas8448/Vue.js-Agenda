<script setup>
defineProps({
    //0000 - 2359
    start: {
        type: Number,
        required: true
    },
    end: {
        type: Number,
        required: true
    }
})
</script>

<template>
    <div class="break">
        <h1 class="title">{{ subject }}</h1>
        <p class="time">{{ start }} - {{ end }}</p>
        <p class="day">{{ day }}</p>
    </div>
</template>

<style scoped>
.break {
    background-color: #f1f1f1;
    border: 1px solid black;
    border-radius: 5px;
    padding: 5px;
    margin: 5px;
    width: 100%;
    height: 50%;
    color: rgb(75, 167, 97);
    ;
}
</style>