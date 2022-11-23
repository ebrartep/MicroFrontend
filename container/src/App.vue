<template>
  <div class="container">
    <div>Name: container</div>
    <Remote1></Remote1>
    <Remote2></Remote2>
  </div>
</template> 

<script>
import { defineAsyncComponent } from "vue";

const Remote1 = defineAsyncComponent(() => import("remote1/Remote1"));
const Remote2 = defineAsyncComponent(() => import("remote2/Remote2"));

  export default {
  name: 'App',
  components: { 
    Remote1,
    Remote2
   },

}
</script>