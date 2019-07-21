<template>
    <div class="layout-view">
        <b-row>
            <b-col style="z-index:1000;">
                <Header />
            </b-col>
        </b-row>
        <b-row no-gutter>
            <b-col cols="2">
                <Sidebar />
            </b-col>
            <b-col cols="10">
                <Content />
            </b-col>
        </b-row>
    </div>
</template>

<script>
import Sidebar from '../components/layout/Sidebar'
import Content from '../components/layout/Content.vue'
import Header from '../components/layout/Header.vue'

export default {
    name: "LayoutView",
    components: {
        Sidebar,
        Content,
        Header
    }
}
</script>

<style scope>
</style>
