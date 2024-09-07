<template>
    <div class="header">
        <h2>Create new booking</h2>
        {{ booking }}
    </div>
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
            <div class="container">
                <label for="total_cost_ex_tax">Total Cost Ex Tax:</label>
                <input type="number" v-model="booking.total_cost_ex_tax">
            </div>
            <div class="container">
                <label for="market_date">Total tax:</label>
                <input type="number" v-model="booking.total_tax">
            </div>
            <div class="container">
                <label for="total_cost_inc_tax">Total cost inc tax:</label>
                <input type="number" v-model="booking.total_cost_inc_tax">
            </div>
            <div class="container">
                <label for="comment">Comment</label>
                <textarea v-model="booking.comment"></textarea>
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
            total_cost_ex_tax:null,
            total_tax:null,
            total_cost_inc_tax:null,
            comment:null,
        })

        return {booking}
    }
}
</script>
