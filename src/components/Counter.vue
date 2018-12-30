<template>
  <div>
      {{ count }}
      <p>
        <button @click="tambah">+</button>
        <button @click="kurang">-</button>
      </p>   
  </div>
</template>


<script>
  export default {
    //props
    props: {
      initCount: Number
    },
    
    //state
    data(){
      return {
        count: 0
      }
    },
    created() {
      this.count = this.initCount
    },
    
    methods: {
      tambah(){
        this.count++
      },
      kurang(){
        this.count--
      }
    },
  }

</script>