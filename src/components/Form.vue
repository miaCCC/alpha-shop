<template>
   <section class="main_form mx-3 mb-8">
    <div>
    <FormAddress />
    </div>

    <div>
    <FormShipment />
    </div>

    <div>
    <FormPayment />
    </div>
   </section>
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