<script setup>
    import {ref} from 'vue'
    const count = ref(0)
</script>

<template>
    <div id="cont_birth">
        <form id="birth_form">
            <div id="inputs">
                <div class="input">
                    <label for="b_day">Day:</label>
                    <input type="number" id="b_day" name="b_day" value="5" min="0" max="31"/>
                </div>
                <div class="input">
                    <label for="b_month">Month:</label>
                    <input type="number" id="b_month" name="b_month" value="12" min="0" max="12"/>
                </div>
                <div class="input">
                    <label for="b_year">Year:</label>
                    <input type="number" id="b_year" name="b_year" value="1990" min="0" max="3000"/>
                </div>
            </div>
            <div class="button-sub">
                <button id="birth_button">submit</button>
            </div>
        </form>
    </div>
</template>

<style scoped>
#birth_form {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    align-items: center;
}

#inputs{
    min-width: 100px;
    width:100%;
}

.input{
    font-size: 1em;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: center;
    margin:1em;
    justify-content: space-between;
    height: 60px;
}
.input input{
    font-size: 1em;
}

#birth_form button{
    font-size: 1.2em;
    background: white;
    border:0;
    border-radius: 1em;
    padding: 0.5em 1em;
    margin: .6em .4em;
}

@media (min-width: 1024px) {
    #inputs{
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
    }
}

</style>