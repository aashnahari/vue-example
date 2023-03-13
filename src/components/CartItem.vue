<script>
    export default{
        emits: ['addOne', 'deleteOne'],
        methods: {
            addOne() {
            quantity++
            //this.$emit('changeData', hotdog.hotdog);
            },
            deleteOne(){
                quantity--
            }
        }
    }    
</script>
<template>
    <div class="item">
        <button @click="addOne">Add One</button>
        <button @click="deleteOne">Delete One</button>
    </div>
    
</template>
  
<style>
.item {
    display: flex;
    align-items: center;
    margin-top: 2rem;
}
</style>
  