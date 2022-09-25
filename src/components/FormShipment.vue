<template>
  <section class="part part-2">
    <div class="main-title my-8">運送方式</div>

    <div class="shipment-container"
      v-for="shipment in shipments"
      :key="shipment.id">
      
      <div class="shipment mt-3 d-flex">
        <input
          name="ta-gender"
          type="radio"
          value="standard"
          @click="shipmentChoice(shipment.fee)"/>
        <div class="shipment-choice">
          <div class="d-flex justify-content-between">
            <label for="">{{shipment.shipment}}</label>
            <div class="price">{{shipment.fee}}</div>
          </div>
          <div class="time">
            <span>{{shipment.time}}</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>


<style scoped>
.shipment {
  position: relative;
  border: 1px solid lightgray;
  border-radius: 5px;
  padding: 1em;
  font-size: 14px;
  font-weight: 500;
  color: black
}
.shipment:hover {
  border: 1px solid black;
}
.shipment-choice {
  width: 100%;
  margin-left: 1rem;
}

</style>

<script>
import { eventBus } from '../main';

const dummyData = {
  shipments: [
    {
      id: 1,
      shipment: '標準運送',
      fee: '免費',
      time: '約3~7個工作天'
    },
    {
      id: 2,
      shipment: 'DHL貨運',
      fee: '500',
      time: '48 小時內送達'
    }
  ]
}

export default {
  data() {
    return {
      shipments: [],
      fee: 0
    }
  },

  methods: {
    fetchShipment() {
      this.shipments = dummyData.shipments

    },
    shipmentChoice(shippingFee) {
        if(shippingFee === '免費') {
          this.fee = 0                  
        } else if (shippingFee === '500') {
          this.fee = 500
        }
        console.log(this.fee)
        eventBus.$emit('after-shipmentChoice',this.fee)
      }
 
  },
  created() {
    this.fetchShipment()
  }
}
</script>
