<template>
    <div>
        {{ booking }}
        <BookingItemForm
        :booking="booking"
        />
        <ActionButton/>
    </div>
</template>

<script >
import { ref } from 'vue';
import ActionButton from '../components/ActionButton.vue';
import BookingItemForm from './components/ItemForm.vue'
export default {
    components: {
        BookingItemForm,
        ActionButton
    },
    setup(){
        const booking = ref({
      stallholder: null,
      market_date: null,
      total_cost_ex_tax: null,
      total_tax: null,
      total_cost_inc_tax: null,
      comment: null,
    });

    return { booking };
    }
}
</script>

