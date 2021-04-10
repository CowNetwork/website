<script lang="ts">
    import { Component, Vue } from "vue-property-decorator";

    import CowNav from "@/fragments/Nav.fragment.vue";

    @Component({
        components: {
            CowNav,
        },
    })
    export default class App extends Vue {

    }
</script>

<template>

    <div id="app" class="text-marine-dark">
        <router-view />
        <cow-nav />
    </div>

</template>

<style lang="scss">

    @import url('https://fonts.googleapis.com/css2?family=Asap:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&family=Caveat:wght@400;500;600;700&family=Lora:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&family=Signika:wght@300;400;500;600;700&display=swap');

</style>