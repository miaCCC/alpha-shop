<template>
      <div class="form-panel left-panel mb-8">
        <div class="form-container">
          <Form-address 
           v-if="step === 1"/>
          <FormShipment v-if="step === 2"/>
          <FormPayment v-if="step === 3"/>
          
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
   props: {
    step: {
      type: Number,
      required: true
    },


  },
  }

  </script>
 