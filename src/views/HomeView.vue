<template>
  <b-container>
    <div class="modal" :id="modal.modalClientId" v-for="employee in modal.data" :key="employee.id" title="employee data" @click.stop>
      <div class="modal-content" v-if="show">
        <div>{{ modal.data.profile_image }}</div>
      </div>
    </div>
  </b-container>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>
