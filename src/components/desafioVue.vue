<template >

      <div>
                <hr>
                <table :style="estilo" >
                    <tbody :class="clase">
                        <tr v-for="item in listado" :key="item.id">
                            <td>{{ item.id }}</td>
                            <td>{{ item.nombre }}</td>
                        </tr>
                    </tbody>
                </table>
                <hr>
            </div>
            

</template>


<script lang="js">

  export default  {
    name: 'desafioVue' ,
    props:{
     listado: Array,
     clase: Object,
     estilo: Object
            },
    mounted () {

    },
    data () {
      return {

      }
    },
    methods: {

    },
    computed: {

    }
}


</script>

<style scoped>
  
</style>
