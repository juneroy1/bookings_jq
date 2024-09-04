<template>
  <div class="about display-flex">
    <h1>List booking page</h1>
    <button class="btn btn-primary" @click="createNewBooking()">Create Booking</button>
    <div class="sizeBox-50"></div>
    <table class="width-100-per">
      <th>Stall holder</th>
      <th>Booked Item</th>
      <th>Quantity</th>
      <th>Total Tax</th>
      <th>Total Cost</th>
      <tr>
        <td>Juneroy</td>
        <td>ITEM 1</td>
        <td>10</td>
        <td>$10.00</td>
        <td>$100.00</td>
      </tr>
      <tr>
        <td>Quinimon</td>
        <td>ITEM 2</td>
        <td>20</td>
        <td>$20.00</td>
        <td>$200.00</td>
      </tr>
    </table>
  </div>
</template>
<script >
import { onMounted, ref } from 'vue';
import '../assets/css/style.css'

export default{
  setup(){
    const bookings = ref([]);

    const createNewBooking = () => {
    }
    onMounted(() =>{
      
    })
    
    return {bookings,createNewBooking}
  },
}

</script>
