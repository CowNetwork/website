<script lang="ts">
    import { Component, Vue } from "vue-property-decorator";

    @Component({ })
    export default class CowNav extends Vue {

    }
</script>

<template>

    <nav class="cow-nav fixed text-white top-0 w-full" role="navigation">
        <div class="flex font-semibold max-w-7xl mx-auto p-4
            xl:px-0">

            <div class="flex items-center space-x-8">
                <a class="flex" href="">
                    <img class="h-8" src="@/assets/logo.png" />
                </a>
            </div>
        </div>
    </nav>

</template>