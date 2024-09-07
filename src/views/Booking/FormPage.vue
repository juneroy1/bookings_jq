<template>
    <div>
        <BookingItemForm/>
        <ActionButton/>
    </div>
</template>

<script >
import ActionButton from '../components/ActionButton.vue';
import BookingItemForm from './components/ItemForm.vue'
export default {
    components: {
        BookingItemForm,
        ActionButton
    },
    setup(){

    }
}
</script>

