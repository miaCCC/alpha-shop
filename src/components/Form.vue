<template>
      <div class="form-panel left-panel mb-8">
        <div class="form-container">
          <Form-address />
          <FormShipment />
          <FormPayment />
          
        </div>
      </div>
</template>
 
<script>
import FormAddress from '../components/FormAddress.vue'
import FormShipment from '../components/FormShipment.vue'
import FormPayment from '../components/FormPayment.vue'



export default {
  components: {
    FormAddress,
    FormShipment,
    FormPayment,
  },
  }

  </script>