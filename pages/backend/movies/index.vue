<template>
  <AppDataTable :header="headers" :data="data" />
</template>

<script>
import axios from 'axios'
import AppDataTable from '../../../components/AppDataTable.vue'
export default {
  name: 'IndexPage',
  layout: 'backend/layout',
  components: {
    AppDataTable,
  },
  head() {
    return {
      title: this.toCapitalize(this.$route.name)+' List',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Know Various '+this.toCapitalize(this.$route.name)+' Name',
        },
      ],
    }
  },
  data() {
    return {
      headers: [],
      data: [],
    }
  },
  async created() {

    const config = {
      headers: {
        Accept: "application/json"
      }
    }

    try {
      const res = await axios.get('https://movies-0623.herokuapp.com/movies', config);
      this.data = res.data
    } catch (error) {
      console.log(error)
    }

    
    this.headers = this.generateTableStructure(this.data[0], 5)
  },
  methods: {
      toCapitalize(word){
          return word[0].toUpperCase() + word.slice(1).toLowerCase()
      },
      generateTableStructure(sampleObj, columLimit = 5){
        let arr = []
        if (sampleObj !== undefined) {
          const firstData = Object.keys(sampleObj)
          for (let i = 0; i < firstData.length; i++) {
            if(i<=columLimit){
              const myKey = firstData[i]
              const obj = {}
              obj.text = this.toCapitalize(myKey)
              obj.value = myKey
              arr.push(obj)
            }else{
              break;
            }
          }
        }
        return arr;
      }
  }
}
</script>

<style lang="scss" scoped></style>
