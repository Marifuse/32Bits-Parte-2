<template>
    <div>
        <header>
            <h1 class="title-store" v-text="title"></h1>
            <h2 class="subtitle-store" v-text="subTitle"></h2>
        </header> 
    </div>
</template>

<script>
import { mapState } from 'vuex'
export default {
    computed: {
        ...mapState(['title', 'subTitle'])
    } 
}
</script>

<style>
    .title-store, .subtitle-store {
        text-align: center;
        padding: 1em;
    }

</style>
