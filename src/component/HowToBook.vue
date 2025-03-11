<script lang="ts" setup></script>

<template>
    <main class="text-container">
        <h2>Bokning</h2>
        <p>Hos SkyVoyage erbjuder vi oförglömliga flygturer med både luftballong och akrobatflyg där du får uppleva världen från ett helt nytt  perspektiv! Oavsett om du vill fira en speciell dag, överraska någon du tycker om eller bara njuta av den magiska känslan av att flyga högt upp i luften, så är det ett äventyr du sent kommer glömma.</p>
        <p>Vi erbjuder både privata och gruppbokningar, vilket gör det perfekt för romantiska utflykter, familjeäventyr, företagsevent eller andra speciella tillfällen.</p>
    </main>
</template>

<style lang="scss" scoped>
    .text-container {
        background-color: $charcoal;
        border-radius: 8px;
        max-width: 900px;
        width: 90%;
        margin: 45px auto;

        h2 {
            font-family: $font-heading2;
            font-size: $mobile-font-size-heading2;
            color: white;
            font-weight: 500;
            padding: 10px 0 0 10px;
        }

        p {
            font-family: $font-body;
            font-size: $mobile-font-size-paragraph;
            color: white;
            font-weight: 200;
            padding: 0 0 10px 10px;
        }
    }

    @media screen and (min-width: 768px) {
        .text-container {

            h2 {
                font-size: $tablet-font-size-heading2;
            }

            p {
                font-size: $tablet-font-size-paragraph;
            }
        }
    }
    @media screen and (min-width: 1024px) {
        .text-container {

            h2 {
                font-size: $desktop-font-size-heading2;
            }
            
            p {
                font-size: $desktop-font-size-paragraph;
            }
        }
    }
</style>