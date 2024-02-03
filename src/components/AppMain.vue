<script>

import AppMainBottom from './AppMainBottom.vue';


export default {
    name: 'AppMain',
    data() {
        return {};
    },
    components: { AppMainBottom }
}
</script>

<template>
    <main>
        <div class="main-top">
            <div class="container">
                <span>Content goes here</span>
            </div>
        </div>
        <AppMainBottom></AppMainBottom>
    </main>
</template>


<style scoped>
.main-top {
    display: flex;
    min-height: 100px;
    background-color: var(--dc-dark);

    & span {
        color: var(--dc-white);
        align-items: center;
        font-weight: 600;
    }
}
</style>