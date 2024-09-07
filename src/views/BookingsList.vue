<template>
  <div class="about display-flex">
    <h1>List booking page</h1>
    <button class="btn btn-primary" @click="createNewBooking()">
      Create Booking
    </button>
    <div class="sizeBox-50"></div>
    <table class="width-100-per">
      <thead>
        <tr>
          <th>Stall holder</th>
          <th>Booked Item</th>
          <th>Quantity</th>
          <th>Total Tax</th>
          <th>Total Cost</th>
        </tr>
      </thead>
      <tbody>
        <tr :key="index" v-for="(booking,index) in bookings">
          <td>Juneroy</td>
          <td>ITEM 1</td>
          <td>10</td>
          <td>$10.00</td>
          <td>$100.00</td>
        </tr>
        
      </tbody>
    </table>
  </div>
</template>
<script>
import { onMounted, ref } from "vue";
import "../assets/css/style.css";
import router from "@/router";

export default {
  setup() {
    const bookings = ref([
      {
        id:1,
        stall_holder:1,
        booking_item:1,
        market_date:1,
        quantity:11,
        total_tax:10.00,
        total_cost:1000.00,
        total_cost_inc_tax:1010.00,
      },
      {
        id:2,
        stall_holder:2,
        booking_item:2,
        market_date:1,
        quantity:5,
        total_tax:10.00,
        total_cost:500.00,
        total_cost_inc_tax:510.00,
      }
    ]);

    const createNewBooking = () => {
      router.push("/booking/create");
    };
    onMounted(() => {});

    return { bookings, createNewBooking };
  },
};
</script>
