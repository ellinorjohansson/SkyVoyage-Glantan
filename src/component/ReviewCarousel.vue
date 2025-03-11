<script lang="ts" setup>
    import { ref } from "vue";

    interface IReview {
        review: string;
        name: string;
         age: number;
    }

    //array med recensionerna
    const reviews = ref<IReview[]>([
     { review: "Superkul. Var vettskrämd men kul var det!", name: "Margareta", age: 56 },
     { review: "Wow, det här vill jag göra igen! Mycket professionell personal!", name: "Anders", age: 41 },
    { review: "Häftig upplevelse men en gång räcker för mig!", name: "Sara", age: 27 },
    ]);

    // Håller koll på vilken recension som visas
    const currentReviewIndex = ref(0);

    // Funktioner för att byta recension
const nextReview = () => {
  // Öka index för nästa recension
  currentReviewIndex.value = (currentReviewIndex.value + 1) % reviews.value.length;
};

const previousReview = () => {
  // Minska index för föregående recension
  currentReviewIndex.value = (currentReviewIndex.value - 1 + reviews.value.length) % reviews.value.length;
};

</script>


<template>
    <section class="review-section">
        <span class="review-header">Så här tyckte våra passagerare!</span>
        <div class="review-container">
            <transition name="fade" mode="out-in">
                <div :key="reviews[currentReviewIndex].review" class="review-text-container">
                    <p class="review-text">"{{ reviews[currentReviewIndex].review }}"</p>
                    <p class="review-author">- {{ reviews[currentReviewIndex].name }}, {{ reviews[currentReviewIndex].age }} år</p>
                </div>
            </transition>
        </div>
        <div class="arrow-container">
            <button  @click="previousReview" aria-label="Föregående recension">
                <i class="fa-solid fa-play fa-rotate-180"></i>
            </button>
            <span>Bläddra för fler recensioner</span>
            <button @click="nextReview" aria-label="Nästa recension">
                <i class="fa-solid fa-play"></i>
            </button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    .review-section {
        height: 250px;
        background-color: $charcoal;
        display: flex;
        color: white;
        font-family: $font-body;
        flex-direction: column;
        padding-left: 5%;
        padding-right: 5%;
        border-radius: 8px;
        margin: 90px 2.5% 60px 2.5%;
        
        .review-header {
            font-family: $font-heading2;
            font-size: $mobile-font-size-heading2;
            margin-top: 15px;
        }

        .review-container {
            text-align: right;

            .review-text {
                font-style: italic;
                font-weight: 200;
                width: 250px;
                margin-left: auto;
            }
        }

        .arrow-container {
            height: 100px;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: space-between;

            button {
                background: none;
                border: none;
            }

            i {
                color: white;
                height: 44px;
                width: 44px;
                display: inline-block;
                font-size: 2rem;
                z-index: 10000;
                position: relative;
                line-height: 44px;


            }
           
        }
    }

//---------För att recensionen ska fadeas ut------------

    .review-container .fade-enter-active, 
.review-container .fade-leave-active {
  transition: opacity 0.2s ease-in-out;
}

.review-container .fade-enter, 
.review-container .fade-leave-to /* .fade-leave-to är för äldre versioner av Vue */ {
  opacity: 0; /* Start opacity för fade-out eller fade-in */
}

.review-container .fade-enter-to {
  opacity: 1; /* När elementet har börjat in-fade */
}

    //tablet
@media screen and (min-width: 768px) {
    .review-section {
        margin-top: 0;
        margin-bottom: 20px;

        .review-header {
            font-size: $tablet-font-size-heading2;
        }

        .review-container {
            width: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;

            .review-text {
                font-size: 1.2rem;
                margin-left: 0;
                width: 100%;
            }
        }
        
        .arrow-container {
            justify-content: center;
            gap: 20px;
        }
    }

}

//desktop
@media screen and (min-width: 1024px) {
    .review-section {
        margin-top: 20px;
        margin-bottom: 60px;

        .review-header {
            font-size: $desktop-font-size-heading2;
        }
    }

}

</style>