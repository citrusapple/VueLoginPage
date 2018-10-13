<template>
    <section>
        <button class="button is-primary is-medium"
            @click="isComponentModalActive = true">
            Launch component modal
        </button>

        <b-modal :active.sync="isComponentModalActive" has-modal-card>
            <ModalForm />
        </b-modal>
    </section>
</template>

<script>
import ModalForm from './components/ModalForm.vue'
    export default {
        components: {
            ModalForm
        },
        data() {
            return {
                isComponentModalActive: false,
                formProps: {
                    email: 'evan@you.com',
                    password: 'testing'
                }
            }
        }
    }
</script>
<style>
body {
  display: grid;
  align-content: center;
  justify-items: center;
}
</style>
