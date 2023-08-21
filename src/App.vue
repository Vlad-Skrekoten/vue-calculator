<script setup>

</script>

<template>
    <main class="container">
        <main class="container">
            <div class="head">
                <label class="switch">
                    <input type="checkbox">
                    <span class="slider"></span>
                </label>
            </div>
            <div class="calculator">
                <div class="numbers">6,291</div>
                <div class="window">
                    <input type="text" class="input">
                </div>
            </div>
            <div class="block_buttons">
                <button class="button button_grey">C</button>
                <button class="button button_grey"><img src="./assets/images/action.svg" alt="action"></button>
                <button class="button button_grey">%</button>
                <button class="button button_blue">÷</button>
                <button class="button">7</button>
                <button class="button">8</button>
                <button class="button">9</button>
                <button class="button button_blue">x</button>
                <button class="button">4</button>
                <button class="button">5</button>
                <button class="button">6</button>
                <button class="button button_blue">-</button>
                <button class="button">1</button>
                <button class="button">2</button>
                <button class="button">3</button>
                <button class="button button_blue">+</button>
                <button class="button">.</button>
                <button class="button">0</button>
                <button class="button"><img src="./assets/images/delete.svg" alt="delete"></button>
                <button class="button button_blue">=</button>
            </div>
        </main>
    </main>
</template>

<style scoped lang="scss">
@import "./assets/scss/main.scss"
</style>
