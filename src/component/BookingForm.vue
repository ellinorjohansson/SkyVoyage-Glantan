<script setup lang="ts">
import { ref, computed} from "vue";


const firstName = ref("");
const lastName = ref("");
const emailAdress = ref("");
const phoneNumber = ref("");
const date = ref("");
const time = ref("");
const quantity = ref<string | number>("");
const age = ref<string | number>("");
const ClientInformation = ref("");

const selectedExperience = ref([]);

const isFormValid = computed(() => {
    
    return (
    firstName.value.trim() !== "" &&
    lastName.value.trim() !== "" &&
    emailAdress.value.trim() !== "" &&
    phoneNumber.value.trim() !== "" &&
    selectedExperience.value.length > 0 && // Minst en checkbox vald
    date.value !== "" &&
    time.value !== "" &&
    Number(quantity.value) > 0 &&
    Number(age.value) > 0
    );
});

function onSubmit() {
    resetForm();
}

function resetForm() {
    firstName.value = "";
    lastName.value = "";
    emailAdress.value = "";
    phoneNumber.value = "";
    date.value = "";
    time.value = "";
    quantity.value = "";
    age.value = "";
    ClientInformation.value = "";
    selectedExperience.value = [];
}

</script>

<template>
    <main class="booking-container">
        <section>
            <h2>Bokningsformulär</h2>
            <p class="booking-p">Vänligen fyll i detta formulär noggrant och sanningsenligt så att vi kan säkerställa att ni får en oförglömlig upplevelse!</p>
        </section>

        <form @submit.prevent="onSubmit">
            <label class="first-name">
                <span>Förnamn</span>
                <input v-model="firstName" type="text">
            </label>

            <label class="last-name">
                <span>Efternamn</span>
                <input v-model="lastName" type="text">
            </label>

            <label class="email-adress">
                <span>Emailadress</span>
                <input v-model="emailAdress" type="email">
            </label>

            <label class="phone-number">
                <span>Telefonnummer</span>
                <input v-model="phoneNumber" type="text">
            </label>

            <fieldset class="selected-experience">
                <legend>Typ av flygupplevelse</legend>

                <div class="checkbox-container option-one">
                    <input type="checkbox" id="option1" v-model="selectedExperience" value="Luftballong, en person">
                    <label for="option1">Luftballong, en person</label>
                </div>

                <div class="checkbox-container option-two">
                    <input type="checkbox" id="option2" v-model="selectedExperience" value="Luftballong, fler än en person">
                    <label for="option2">Luftballong, fler än en person</label>
                </div>

                <div class="checkbox-container option-three">
                    <input type="checkbox" id="option3" v-model="selectedExperience" value="Akrobatflyg, en person">
                    <label for="option3">Akrobatflyg, en person</label>
                </div>

                <div class="checkbox-container option-four">
                    <input type="checkbox" id="option4" v-model="selectedExperience" value="Akrobatflyg, fler än en person">
                    <label for="option4">Akrobatflyg, fler än en person</label>
                </div>
            </fieldset>


            <label class="date">
                <span>Datum</span>
                <input v-model="date" type="date">
            </label>

            <label class="time">
                <span>Tid</span>
                <input v-model="time" type="time">
            </label>

            <label class="quantity">
                <span>Hur många är ni?</span>
                <input v-model="quantity" type="number">
            </label>

            <label class="age">
                <span>Ålder</span>
                <input v-model="age" type="number">
            </label>

            <label class="info-container">
                <span>Övrig information</span>
                <p class="info-example">Till exempel; underliggande sjukdomar, höjdrädsla, etc</p>
                <textarea v-model="ClientInformation" class="large-input" rows="6" cols="150"></textarea>            
                </label>

            <div class="button-container">
                <input class="submit-btn" type="submit" value="Skicka in" :disabled="!isFormValid">
                <input class="reset-btn" type="reset" value="Rensa" >
            </div>
        </form>
    </main>
</template>


<style lang="scss" scoped>
    .booking-container {
        background-color: $charcoal;
        border-radius: 8px;
        max-width: 900px;
        width: 90%;
        margin: 45px auto;

        section {
            background-color: $paynes-gray;
            border-radius: 8px;

            h2 {
                font-family: $font-heading2;
                font-size: $mobile-font-size-heading2;
                color: white;
                padding: 10px;
                font-weight: 500;
                margin: 0;
            }

            .booking-p {
                font-family: $font-body;
                font-size: $mobile-font-size-paragraph;
                color: white;
                font-weight: 200;
                padding: 10px;
                margin: 0;
            }
        }
        

        label {
            margin: 20px;
            display: flex;
            flex-direction: column;
            gap: 5px;
            color: white;
            font-family: $font-heading2;
            font-size: $mobile-font-size-heading2;

            input{
                width: 300px;
                height: 40px;
                border-radius: 8px;
                background-color: white;
                border: none;
                font-size: 1rem;
                font-family: $font-heading2;
            }
        }

        fieldset {
            border: none;
            margin: 20px 0;
            padding: 10px;
            color: white;
            font-family: $font-heading2;

            legend {
                font-size: $mobile-font-size-heading2;
                font-weight: bold;
                margin-bottom: 10px;
            }

            .checkbox-container {
                align-items: center;
                display: flex;
            }

            input[type="checkbox"] {
                width: 18px;
                height: 18px;
                accent-color: $coral; 
            }
        }

        .info-container {
            .info-example {
                padding: 0;
                font-size: $mobile-font-size-paragraph;
                font-family: $font-body;
                font-weight: 200;
                max-width: 200px; 
                word-wrap: break-word;
            }

            .large-input {
                width: 300px;  
                height: 60px;  
                font-size: 1rem;
                padding: 10px;
                border-radius: 8px;
            }
        }
        
        .button-container{
            .submit-btn {
                margin: 0 33px 20px 20px;
                font-weight: normal;
            }

            .reset-btn {
                cursor: pointer;
            }
        
            input {
                font-family: $font-body;
                font-size: $font-size-button;
                width: 110px;
                height: 44px;
                border-radius: 8px;
                border: none;
                box-shadow: 0px 4px 4px 0px #00000040;
                background-color: $coral;
                color: black;

                &:disabled {
                    background-color: #f57e4b91;
                }
            }
        }
    }

    @media screen and (min-width: 768px) {
        .booking-container {
            section {

                h2 {
                font-size: $tablet-font-size-heading2;
                }

                .booking-p {
                    font-size: $tablet-font-size-paragraph;
                }
            }
            
            form {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                grid-template-rows: auto;

                .first-name{
                  grid-column: 1;
                  grid-row: 1;
                }

                .last-name {
                    grid-column: 2;
                    grid-row: 1;
                }

                .email-adress{
                    grid-column: 1/ span 2;
                    grid-row: 2;
                    input{
                        width: 400px;
                    }
                }

                .phone-number {
                    grid-column: 1 / span 2;
                    grid-row: 3;
                    input{
                        width: 400px;
                    }
                }

                .selected-experience{
                    grid-column: 1 / span 2;
                    grid-row: 4;
                }
                    
                fieldset {
                    display: grid;
                    grid-template-columns: repeat(2, 1fr);
                    grid-template-rows: auto;

                    legend {
                        grid-column: 1 / 2;
                        grid-row: 1;
                    }

                    input[type="checkbox"] {
                        width: 35px;
                        height: 35px;
                    }

                    .option-one {
                        grid-column: 1;
                        grid-row: 2;
                    }

                    .option-two {
                        grid-column: 2;
                        grid-row: 2;
                    }

                    .option-three {
                        grid-column: 1;
                        grid-row: 3;
                    }

                    .option-four {
                        grid-column: 2;
                        grid-row: 3;
                    }
                }

                .date {
                    grid-column: 1;
                    grid-row: 7;
                }

                .time {
                    grid-column: 2;
                    grid-row: 7;
                }

                .quantity {
                    grid-column: 1;
                    grid-row: 8;      
                }

                .age {
                    grid-column: 2;
                    grid-row: 8;
                }

                .info-container {
                    grid-column: 1 / span 2;
                    grid-row: 9;
                    .large-input {
                        width: 400px;
                        height: 90px;
                    }
                }

                .button-container {
                    grid-column: 1 / span 2;
                    grid-row: 10;
                    
                    .submit-btn, .reset-btn{
                        width: 195px;
                    }
                }
            }
        }
    }
    
    @media screen and (min-width: 1024px) {
        .booking-container {
            section {

                h2 {
                    font-size: $desktop-font-size-heading2;
                }
                
                .booking-p {
                    font-size: $desktop-font-size-paragraph;
                }
            }
        }
    }
</style>
