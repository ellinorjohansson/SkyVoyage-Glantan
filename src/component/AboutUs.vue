<script lang="ts" setup></script>

<template>
    <main>
        <h2>Om oss</h2>
        <p>Välkommen till SkyVoyage – din portal till oförglömliga flygupplevelser! Vi brinner för att ge våra kunder chansen att uppleva himlen på ett unikt och spännande sätt, oavsett om det handlar om adrenalinfyllda akrobatflygningar eller rofyllda luftballongsturer.</p>
        <p>Våra samarbetspartners är erfarna piloter och ballongförare som garanterar en trygg och oförglömlig upplevelse, oavsett vilket äventyr du väljer. Oavsett om du vill känna G-krafterna i en loop eller sväva stilla över landskapet i en luftballong, har vi något för dig.</p>
        <p>Låt oss hjälpa dig att ta ditt nästa äventyr till nya höjder – bokning och mer information hittar du här på vår sida. Vi ser fram emot att ge dig en upplevelse du sent kommer att glömma!</p>
    </main>
</template>

<style lang="scss" scoped>
    main {
        background-color: $charcoal;
        border-radius: 8px;
        max-width: 900px;
        width: 90%;
        margin: 45px auto;

        h2 {
            font-family: $font-heading2;
            font-size: $mobile-font-size-heading2;
            color: white;
            padding: 10px;
            font-weight: 500;
            margin: 0;
        }

        p {
            font-family: $font-body;
            font-size: $mobile-font-size-paragraph;
            color: white;
            font-weight: 200;
            padding: 10px;
            margin: 0;
        }
    }
    @media screen and (min-width: 768px) {
        main {

            h2 {
                font-size: $tablet-font-size-heading2;
            }

            p {
                font-size: $tablet-font-size-paragraph;
            }
        }
    }
    @media screen and (min-width: 1024px) {
        main {

            h2 {
                font-size: $desktop-font-size-heading2;
            }
            
            p {
                font-size: $desktop-font-size-paragraph;
            }
        }
    }
</style>