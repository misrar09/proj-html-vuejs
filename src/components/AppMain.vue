<script>
import { store } from "../store.js" //state management
import register from "../debug" //per debuggare il componente da console

export default {
    name: "AppMain",
    data() {
        return {
            store
        }
    },
    methods: {
        doThings() {
            console.log("AppComponent does things");
        }
    },
    mounted() {
        register(this); //per debuggare il componente da console
        this.doThings();
    }
}
</script>

<template>
    <div class="container">
        <section class=" row jumbotron">
            <h6>Certified fitness professionals</h6>
        </section>
        <section class=" row services"></section>
        <section class=" row online_advice"></section>
        <section class=" row mailing_list"></section>
        <section class=" row information"></section>
        <section class=" row articles"></section>
        <section class=" row call_to_action"></section>
        <section class=" row other_info"></section>
        <section class=" row workout_of_the_day"></section>


    </div>
</template>

<style scoped lang="scss">
// importo variabili
// @use './styles/partials/variables' as *;

// ...qui eventuale SCSS di AppComponent
</style>