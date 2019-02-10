<template>
  <f7-page>
    <div style="width: 100%">
      <vue-phone-number-input v-model="phoneNumber" />
    </div>
  </f7-page>
</template>
<script>
import VuePhoneNumberInput from 'vue-phone-number-input'

export default {
  name: 'PhonePage',
  components: {
    VuePhoneNumberInput
  },
  data () {
    return {
      phoneNumber: null
    }
  }
}
</script>
