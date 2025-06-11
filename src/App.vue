<template>
    <div>
        <p>counterL {{ counter }}</p>
        <div class="d-flex gap-1">
            <button v-on:click="inc" class="btn btn-success">inc</button>
            <button v-on:click="dsc" class="btn btn-danger">dsc</button>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            counter: 2,
        }
    },
    methods:{
        inc(){
            this.counter ++
        },
        dsc(){
            if(this.counter <= 0){
                return this.counter
            }else{

                this.counter --
            }
        }
    }
}
</script>

<style>
</style>