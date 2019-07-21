<template>
    <div>
        <b-container>
            <!-- <router-view/> -->
            <hello-world />
        </b-container>
    </div>
</template>

<script>

import HelloWorld from '../HelloWorld.vue'
export default {
    name: "Content",
    components: {
        HelloWorld
    }
}
</script>

<style>

</style>
