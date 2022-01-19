<template>
    <Header title="RememberMe"></Header>
    <stored-resources :resources="storedResurces"></stored-resources>
</template> 

<script>
import StoredResources from './components/resources/StoredResources'
import Header from './components/layouts/Header'

export default {
    components: {
        StoredResources,
        Header
    },
    data() {
        return {
            storedResurces: [
                {
                    id: 'official-guide',
                    title: 'Official Guide',
                    description: 'The official Vue.js documentation.',
                    link: 'https://vuejs.org'
                },
                {
                    id: 'google',
                    title: 'Google',
                    description: 'Learn to google...',
                    link: 'https://google.com'
                }
            ]
        }
    }
}
</script>

<style>
    @import 'scss/style.scss';
</style>