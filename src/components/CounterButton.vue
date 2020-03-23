<template>
    <div>
        <button v-on:click='decrement()'>-</button>
        <label>&nbsp;{{counter}}&nbsp;</label>
        <button v-on:click='increment()'>+</button>
    </div>
</template>

<script>

export default {
    data(){
        return{
            counter:0
        }
    },
    methods:{
        decrement(){
            if(this.counter>0) {
                this.counter = this.counter - 1
                return this.counter;
            } else
                return this.counter;
        },
        increment(){
            this.counter = this.counter + 1;
            return this.counter;
        }
    }
}
</script>