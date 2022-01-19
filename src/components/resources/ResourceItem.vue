<template>
    <section>
        <base-card>
            <div class="basecard-header">
                <h2>{{ title }}</h2>
                <base-button mode="flat">Delete</base-button>
            </div>
            <p>{{ description }}</p>
            <nav>
                <a :href="link">View Resource</a>
            </nav>
        </base-card>
    </section>
</template>

<script>
import BaseButton from "../UI/BaseButton.vue"

export default{
    components: { BaseButton },
    props: ['title', 'description', 'link'],
}
</script>

<style lang="scss" scoped>

</style>