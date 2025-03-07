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
        <span class="review-header">Så här tyckte våra passagerare!</span>
        <div class="arrow-container">
            <i class="fa-solid fa-play fa-rotate-180"></i>
            <span>Bläddra för fler recensioner</span>
            <i class="fa-solid fa-play"></i>
        </div>
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
        color: white;

        .review-header {
            font-family: $font-heading2;
            font-size: $mobile-font-size-heading2
        }

        .arrow-container {
            width: 100px;
            height: 100px;
            position: relative;

            i {
                color: white;
                height: 44px;
                width: 44px;
                display: inline-block;
                font-size: 2rem;
                z-index: 10000;
                position: relative;


            }
        }
    }

    //tablet
@media screen and (min-width: 768px) {
    
}

//desktop
@media screen and (min-width: 1024px) {

}

</style>