<template>
    <div class="calculator">
        <div class="display">display</div>
        <div>C</div>
        <div>?</div>
        <div>%</div>
        <div>÷</div>
        <div>7</div>
        <div>8</div>
        <div>9</div>
        <div>×</div>
        <div>4</div>
        <div>5</div>
        <div>6</div>
        <div>-</div>
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>+</div>
        <div>+/-</div>
        <div>0</div>
        <div>.</div>
        <div>=</div>
    </div>
</template>

<script>
export default {
    name: 'Calculator',
}
</script>

<style scoped>
.calculator {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-auto-rows: minmax(50px, auto);
}

.display {
    grid-column-start: 1;
    grid-column-end: 5;
    background-color:cornsilk ;
}
</style>