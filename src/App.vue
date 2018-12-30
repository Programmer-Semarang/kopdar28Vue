<template>
  <div>
        <counter :initCount="count" />
        <counter :initCount="count" :class="{warning: this.error < 0}" />
  </div>
</template>


<script>
  import Counter from "./components/Counter";

  export default {
    components: { Counter },

    data(){
      return{
        count:5,
        error:0
      }
    }
    
  }
</script>