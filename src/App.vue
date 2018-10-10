<template>
    <section>
        <button class="button is-primary is-medium"
            @click="isComponentModalActive = true">
            Launch component modal
        </button>

        <b-modal :active.sync="isComponentModalActive" has-modal-card>
            <modal-form v-bind="formProps"></modal-Form>
        </b-modal>
    </section>
</template>

<script>
import ModalForm from './components/ModalForm.vue'

export default {
  name: 'App',
  components: {
    ModalForm
  }
}
</script>

<style>

</style>
