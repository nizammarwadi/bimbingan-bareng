<template>
    <div class="container">
        <button class="button" @click.prevent="$emit ('klik-button')">{{titleBtn}}</button>
    </div>
</template>

<script>
export default {
    props: {
        titleBtn: {
            type: String,
            default: 'Submit'
        }
    }

}
</script>

<style>

</style>