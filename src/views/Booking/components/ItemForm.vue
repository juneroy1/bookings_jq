<template>
    <div>
        {{ test }}
    </div>
</template>

<script>
export default {
    name: "BookingItemForm",
    setup () {
        const test = 'hello test'

        return {test}
    }
}
</script>

<style lang="scss" scoped>

</style>