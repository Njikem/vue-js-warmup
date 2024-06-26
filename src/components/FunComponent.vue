<template>
    <div>
     <h4>This is fun</h4>


   <div>
      <button @click="buttonClicked($event)">Clicked</button>
   </div>

   <div v-for="(secret, i) in secret" :key="i" @click="textColor($event)">

     <p>{{secret.name}}</p>


   </div>

    </div>
</template>

<script>
    export default {
    name: 'FunComponent',
    components: {

    },

    data() {
        return {

           secret: [
            {
                name: 'Johny', 

            },

            {
                name: 'Mauby', 

            },

            {
                name: 'Rose', 

            },

            {
                name: 'Anas', 

            }
        
           ]
          
        }
    },


    methods: {
        buttonClicked(event) {
            console.log('buttonClicked', event);

            event.target.style.backgroundColor = 'red';
            event.target.style.color = 'green';
            
            document.body.style.backgroundColor = 'blue';
        },

        textColor(event){
          console.log(event)
          event.target.style.color = 'pink';
        }
    },
    }
</script>

<style lang="scss" scoped>

</style>