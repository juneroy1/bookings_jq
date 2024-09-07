<template>
    <div class="header">
        <h2>Create new booking</h2>
    </div>
    {{ booking }}
        <div class="form">
            <div class="container">
                <label for="stallholder">Stallholder:</label>
                <select name="stallholder" v-model="booking.stallholder" id="stallholder">
                    <option value="1">Juneroy</option>
                    <option value="2">Quinimon</option>
                    <option value="3">Derano</option>
                </select>
            </div>
            <div class="container">
                <label for="market_date">Market date:</label>
                <select name="market_date" v-model="booking.market_date" id="market_date">
                    <option value="1">Market 1</option>
                    <option value="2">Market 2</option>
                    <option value="3">Market 3</option>
                </select>
            </div>
        </div>
</template>

<script>
import { ref } from 'vue';

export default {
    name: "BookingItemForm",
    setup () {
        
        const booking = ref({
            stallholder:null,
            market_date:null,
        })

        return {booking}
    }
}
</script>
