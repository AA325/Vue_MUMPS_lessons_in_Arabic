<template>
<div>
    <q-input outlined v-model="input" label="Simple Input Box" />
  <ul>
      <li v-for="item in data" :key="item">
          {{item}}
      </li>    
  </ul>
     <q-btn color="secondary" label="Send to Server and Get Data" @click="sendDataToServer"/>
  </div>
</template>
<script>

export default {
    data() {
        return {
            data:[],
            input:''
        }
    },
    methods:{
       async sendDataToServer(){
        let data = await this.$M('EXAMPLE1^QDEMO',{
            param: this.input
        })
       this.data = data.data
       }
    }
}
</script>
