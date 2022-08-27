<!--<template>
  <div>
    <NuxtWelcome />
  </div>
</template>-->



<template>
    <div id="counter">
        <button @click="decrement">-</button>
        <span>{{ num }} </span>
        <button @click="increment">+</button>
    </div>
</template>

<script>
    export default {
        name: 'Counter',
        data() {
            return {
                num: 0,
            }
        },
        methods: {
            increment: function () {
                this.num++;
            },
            decrement: function () {
                this.num--;
            }
        }
    }
</script>

<style>
#counter {
  display: flex;
  text-align: center;
}
button {
  border-radius: 50%;
  width: 3rem;
  height: 3rem;
  cursor: pointer;
}
span{
  width: 3em;
  height: 3rem;
  line-height: 3rem;
}
</style>
