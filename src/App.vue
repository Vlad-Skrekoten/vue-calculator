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
                <button class="button button_grey">
                    <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M22.8321 7.5547L23.3867 6.72265L21.7226 5.61325L21.1679 6.4453L9.16795 24.4453L8.61325 25.2774L10.2773 26.3868L10.8321 25.5547L22.8321 7.5547ZM9 6V7V9H11H12V11H11H9V13V14H7V13V11H5H4V9H5H7V7V6H9ZM21 21H20V23H21H27H28V21H27H21Z"
                            fill="white" />
                    </svg>
                </button>
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
                <button class="button">
                    <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M10.5858 7H11H27H28V8V24V25H27H11H10.5858L10.2929 24.7071L2.29289 16.7071L1.58578 16L2.29289 15.2929L10.2929 7.29289L10.5858 7ZM11.4142 9L4.41421 16L11.4142 23H26V9H11.4142ZM15 11.5858L15.7071 12.2929L18 14.5858L20.2929 12.2929L21 11.5858L22.4142 13L21.7071 13.7071L19.4142 16L21.7071 18.2929L22.4142 19L21 20.4142L20.2929 19.7071L18 17.4142L15.7071 19.7071L15 20.4142L13.5858 19L14.2929 18.2929L16.5858 16L14.2929 13.7071L13.5858 13L15 11.5858Z"
                            fill="white" />
                    </svg>
                </button>
                <button class="button button_blue">=</button>
            </div>
        </main>
    </main>
</template>

<style scoped lang="scss">
@import "./assets/scss/main.scss"
</style>
