<script>
    export default{
        emits: ['addOne', 'deleteOne'],
        methods: {
            addOne() {
            console.log('addOne in cartitem')
            this.$emit('addOne');
            },
            deleteOne(){
            this.$emit('deleteOne');
            }
        }
    }    
</script>
<template>
    <div>
        <slot></slot>
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
  