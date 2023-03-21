<template>
    <div>
        <h2>About</h2>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iure ducimus corrupti fugiat, quod quaerat nam officia delectus asperiores vitae deleniti nobis cumque architecto voluptatem. Nihil, error aliquam. Nihil, modi ipsa.</p>
        <div>{{ data }}</div>
    </div>
</template>

<script setup>
    const { data } = await useFetch('/api/currency/GBP');
</script>

<style scoped>
    h2{
        margin-bottom: 20px;
        font-size: 36px;
    }

    p{
        margin: 20px 0;
    }
</style>