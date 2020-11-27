<template>
  <div class="container">
    <button class="button" @click="$emit('click-button')" >{{ titleButton }}</button>
  </div>
</template>

<script>
export default {
    props:{
        titleButton:{
            type: String,
            default: 'submit'
        }
    }
}
</script>

<style>

</style>