<template>
  <div class="home">
    <FunComponent/>
  </div>
</template>

<script>
// @ is an alias to /src

import FunComponent from '@/components/FunComponent.vue'
export default {
  name: 'HomeView',
  components: {
  FunComponent
  }
}
</script>
