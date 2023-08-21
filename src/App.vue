<script>
export default {
    data() {
        return {
            result: '',
        }
    },

    methods: {
        input: function (char) {
            this.result = this.result.toString();
            this.result += char;
        },

        deleted: function () {
            this.result = this.result.slice(0, -1);
        },

        reset: function () {
            this.result = '';
        },

        step: function () {
            this.result += this.result ** this.result[this.result.length - 1];
        },

        calc: function () {
            this.result = eval(this.result);
        }
    }
}
</script>

<template>
    <main class="container">
        <main class="container">
            <!-- <div class="head">
                <label class="switch">
                    <input type="checkbox">
                    <span class="slider"></span>
                </label>
            </div> -->
            <div class="calculator">
                <!-- <div class="numbers">{{ result }}</div> -->
                <div class="window">
                    <input type="text" class="input" @keyup.enter="calc" v-model="result" placeholder="0">
                </div>
            </div>
            <div class="block_buttons">
                <button v-on:click="reset()" class="button button_grey">C</button>
                <button v-on:click="input('**')" class="button button_grey">^</button>
                <button v-on:click="input('00')" class="button button_grey">00</button>
                <button v-on:click="input('/')" class="button button_blue">÷</button>
                <button v-on:click="input(7)" class="button">7</button>
                <button v-on:click="input(8)" class="button">8</button>
                <button v-on:click="input(9)" class="button">9</button>
                <button v-on:click="input('*')" class="button button_blue">x</button>
                <button v-on:click="input(4)" class="button">4</button>
                <button v-on:click="input(5)" class="button">5</button>
                <button v-on:click="input(6)" class="button">6</button>
                <button v-on:click="input('-')" class="button button_blue">-</button>
                <button v-on:click="input(1)" class="button">1</button>
                <button v-on:click="input(2)" class="button">2</button>
                <button v-on:click="input(3)" class="button">3</button>
                <button v-on:click="input('+')" class="button button_blue">+</button>
                <button class="button">.</button>
                <button v-on:click="input(0)" class="button">0</button>
                <button v-on:click="deleted()" class="button">
                    <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M10.5858 7H11H27H28V8V24V25H27H11H10.5858L10.2929 24.7071L2.29289 16.7071L1.58578 16L2.29289 15.2929L10.2929 7.29289L10.5858 7ZM11.4142 9L4.41421 16L11.4142 23H26V9H11.4142ZM15 11.5858L15.7071 12.2929L18 14.5858L20.2929 12.2929L21 11.5858L22.4142 13L21.7071 13.7071L19.4142 16L21.7071 18.2929L22.4142 19L21 20.4142L20.2929 19.7071L18 17.4142L15.7071 19.7071L15 20.4142L13.5858 19L14.2929 18.2929L16.5858 16L14.2929 13.7071L13.5858 13L15 11.5858Z"
                            fill="white" />
                    </svg>
                </button>
                <button v-on:click="calc()" class="button button_blue">=</button>
            </div>
        </main>
    </main>
</template>

<style scoped lang="scss">
@import "./assets/scss/main.scss"
</style>
