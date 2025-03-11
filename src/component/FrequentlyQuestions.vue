<script lang="ts" setup></script>

<template>
    <main class="questions-container">
        <h2>Vanliga frågor:</h2>
        <section>
            <h3>Är det säkert att åka luftballong?</h3>
            <p>-Ja, luftballongflyg är en säker aktivitet. Piloterna är certifierade och följer strikta säkerhetsregler. Ballongerna genomgår regelbundna säkerhetskontroller.</p>
        </section>
        <section>
            <h3>Vad händer om det regnar eller blåser mycket?</h3>
            <p>- Vid dåligt väder, som stark vind eller regn, ställs flygningen in av säkerhetsskäl. Du får då möjlighet att boka om din tur.</p>
        </section>
        <section>
            <h3>Kan man boka en privat luftballongtur?</h3>
            <p>- Ja, det går att boka en privat tur, vilket är ett populärt val för speciella tillfällen som födelsedagar eller bröllop.</p>
        </section>
        <section>
            <h3>Vad innebär akrobatflyg?</h3>
            <p>- Akrobatflyg innebär att flygplanet utför olika stunts, som loopar, spiraler eller fartfyllda manövrar i luften. Det är en adrenalinfylld    upplevelse för dem som söker något extra. </p>
        </section>
        <section>
            <h3>Behöver man erfarenhet för att prova akrobatflyg?</h3>
            <p>- Nej, du behöver ingen tidigare erfarenhet av flygning för att prova akrobatflyg. Piloten tar hand om alla manövrer och du får en säker och kontrollerad upplevelse.</p>
        </section>
        <section>
            <h3>Vad händer om jag ångrar mig? Kan jag avboka?</h3>
            <p>- Ja, du kan avboka utan kostnad fram till två veckor innan din flygning. Om du avbokar inom en vecka före flygningen, kommer en avbokningsavgift på 50% av flygkostnaden att debiteras. Om du avbokar senare eller inte dyker upp, debiteras hela kostnaden för flygningen.</p>
        </section>
        <section>
            <h3>Vad händer om jag blir illamående under flygningen?</h3>
            <p>- Det är inte ovanligt att vissa människor känner sig illamående under akrobatflyg. Det är viktigt att du informerar piloten om eventuella problem, och de kan anpassa flygningen för att hjälpa till att minimera obehaget.</p>
        </section>
        <section>
            <h3>Finns det ålders- eller hälsokrav för att prova akrobatflyg?</h3>
            <p>- Vi rekommenderar att du är minst 18 år och har en god allmän hälsa. Det kan också finnas särskilda rekommendationer för personer med hjärtproblem eller andra hälsobesvär.</p>
        </section>
    </main>
</template>

<style lang="scss" scoped>
    .questions-container {
        background-color: $charcoal;
        border-radius: 8px;
        max-width: 900px;
        width: 90%;
        margin: 45px auto;
        padding-bottom: 10px;

        h2 {
            color: white;
            font-family: $font-heading2;
            font-size: $mobile-font-size-heading2;
            font-weight: 500;
            padding: 10px;
        }

        h3 {
            color: white;
            font-family: $font-body;
            font-size: $mobile-font-size-heading3;
            font-weight: 450;
            padding-left: 10px;
        }

        p {
            color: white;
            font-family: $font-body;
            font-size: $mobile-font-size-paragraph;
            font-weight: 200;
            padding-left: 10px;
        }

        section {
            margin-bottom: 30px;
        }
    }

    @media screen and (min-width: 768px) {
        .questions-container {

            h2 {
                font-size: $tablet-font-size-heading2;
            }

            p {
                font-size: $tablet-font-size-paragraph;
            }
        }
    }
    
    @media screen and (min-width: 1024px) {
        .questions-container {

            h2 {
                font-size: $desktop-font-size-heading2;
            }

            p {
                font-size: $desktop-font-size-paragraph;
            }
        }
    }
</style>