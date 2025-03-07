<script lang="ts" setup>
    import { ref } from "vue";

    //array med recensionerna
    const reviews = ref([
        { review: "Superkul. Var vettskrämd men kul var det!",
            name: "Margareta",
            age: 56
        },
        { review: "Wow, det här vill jag göra igen! Mycket professionell personal!",
            name: "Anders",
            age: 41
        },
        { review: "Häftig upplevelse men en gång räcker för mig!",
            name: "Sara",
            age: 27
        },
    ]);
</script>


<template>
    <section class="review-section">

    </section>
</template>

<style lang="scss" scoped>
    .review-section {
        height: 250px;
        width: 95%;
        margin-top: 90px;
        margin-bottom: 60px;
        background-color: $charcoal;
        display: flex;
    }

    //tablet
@media screen and (min-width: 768px) {
    
}

//desktop
@media screen and (min-width: 1024px) {

}

</style>