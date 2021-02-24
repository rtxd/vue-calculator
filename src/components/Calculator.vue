<template>
    <div class="calculator">
        <div class="display">{{display}}</div>
        <div class="button operator">C</div>
        <div class="button operator">+/-</div>
        <div class="button operator">%</div>
        <div class="button operator">÷</div>
        <div class="button">7</div>
        <div class="button">8</div>
        <div class="button">9</div>
        <div class="button operator">×</div>
        <div class="button">4</div>
        <div class="button">5</div>
        <div class="button">6</div>
        <div class="button operator">-</div>
        <div class="button">1</div>
        <div class="button">2</div>
        <div class="button">3</div>
        <div class="button operator">+</div>
        <div class="button zero">0</div>
        <div class="button ">.</div>
        <div class="button operator">=</div>
    </div>
</template>

<script>
export default {
    name: 'Calculator',
    data() {
        return {
            display: "0"
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
    background-color:cornsilk ;
}

.operator {
    background-color: rgba(255, 209, 5, 0.6);
}
.operator:hover {
    background-color: rgba(255, 209, 5, 0.3);
}
</style>