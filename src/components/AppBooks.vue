<script>
export default {
    name: 'AppBooks',
    props: {
        src: String,
        text: String
    },
    data() {
        return {

        }
    }
}
</script>
<template>
    <div class="book">
        <img :src="src" alt="">
        <span>{{ text }}</span>
    </div>
</template>


<style scoped>
.book {
    & span {
        text-transform: uppercase;
        color: var(--dc-white);
        font-size: 10px;
        font-weight: 600;
    }

    & img {
        aspect-ratio: 1;
        height: 130px;
    }
}
</style>