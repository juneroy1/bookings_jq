<template>
    <div class="header">
        <h2>Create new booking</h2>
    </div>
        <div class="form">
            <div class="container">
                <label for="stallholder">Stallholder:</label>
                <select name="stallholder" id="stallholder">
                    <option value="1">Juneroy</option>
                    <option value="2">Quinimon</option>
                    <option value="3">Derano</option>
                </select>
            </div>
            <div class="container">
                <label for="market_date">Market date:</label>
                <select name="market_date" id="market_date">
                    <option value="1">Market 1</option>
                    <option value="2">Market 2</option>
                    <option value="3">Market 3</option>
                </select>
            </div>
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
