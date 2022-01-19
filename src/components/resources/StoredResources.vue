<template>
    <main>
        <resource-item
            v-for="res in resources"
            :key="res.id"
            :title="res.title"
            :description="res.description"
            :link="res.link"
        ></resource-item>
    </main>
</template>

<script>
import ResourceItem from "./ResourceItem"

export default {
    name: 'StoredResources',
    props: ['resources'],
    components: {
        ResourceItem
    }
}
</script>

<style lang="scss" scoped>

</style>