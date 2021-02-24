<template>
    <div class="calculator">
        <div class="display">{{display}}</div>
        <div @click="clear" class="button operator">C</div>
        <div class="button operator">+/-</div>
        <div @click="append('%')" class="button operator">%</div>
        <div @click="append('÷')" class="button operator">÷</div>
        <div @click="append('7')" class="button">7</div>
        <div @click="append('8')" class="button">8</div>
        <div @click="append('9')" class="button">9</div>
        <div @click="append('×')" class="button operator">×</div>
        <div @click="append('4')" class="button">4</div>
        <div @click="append('5')" class="button">5</div>
        <div @click="append('6')" class="button">6</div>
        <div @click="append('-')" class="button operator">-</div>
        <div @click="append('1')" class="button">1</div>
        <div @click="append('2')" class="button">2</div>
        <div @click="append('3')" class="button">3</div>
        <div @click="append('+')" class="button operator">+</div>
        <div @click="append('0')" class="button zero">0</div>
        <div @click="append('.')" class="button">.</div>
        <div class="button operator">=</div>
    </div>
</template>

<script>
export default {
    name: 'Calculator',
    data() {
        return {
            display: ""
        }
    },
    methods: {
        clear() {
            this.display = '';
        },
        append(number) {
            this.display = this.display.concat(number);
        }
    }
}
</script>

<style scoped>
.calculator {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-auto-rows: minmax(70px, auto);
}

.button {
    background-color: floralwhite;
    border: 1px solid rgb(233, 230, 188);
    align-items: center;
    justify-items: center;
    cursor: pointer;
}

.button:hover {
    background-color: rgba(255, 250, 240, 0.3);
}

.button:active {
    transform: scale(0.97);
}

.zero {
    grid-column-start: 1;
    grid-column-end: 3;
}

.display {
    grid-column-start: 1;
    grid-column-end: 5;
    text-align: end;
    background-color:cornsilk ;
}

.operator {
    background-color: rgba(255, 209, 5, 0.6);
}
.operator:hover {
    background-color: rgba(255, 209, 5, 0.3);
}
</style>