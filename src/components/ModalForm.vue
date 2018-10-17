<template>
            <form @submit.prevent="NewUserInfo">
                <div class="modal-card" style="width: 425px">
                    <header class="modal-card-head">
                        <p class="modal-card-title">Signup</p>
                    </header>
                    <section class="modal-card-body">
                        <b-field label="FirstName">
                            <b-input
                                type="firstname"
                                :value="firstname"
                                placeholder="Your First Name"
                                required
                                v-model="firstname">
                            </b-input>
                        </b-field>
                        <b-field label="LastName">
                            <b-input
                                type="lastname"
                                :value="lastname"
                                placeholder="Your Last Name"
                                required
                                v-model="lastname">
                            </b-input>
                        </b-field>
                        <b-field label="Email">
                            <b-input
                                type="email"
                                :value="email"
                                placeholder="Your email"
                                required
                                v-model="email">
                            </b-input>
                        </b-field>

                        <b-field label="Password">
                            <b-input
                                type="password"
                                :value="password"
                                password-reveal
                                placeholder="Your password"
                                required
                                v-model="password">
                            </b-input>
                        </b-field>
                        <!-- why does the arrows not show up? I don't think there's any CSS clashes? -->
                        <b-field label="Birthdate">
                            <b-datepicker
                                placeholder="Click to select..."
                                icon="calendar-today"
                                v-model="birthdate"
                                >
                            </b-datepicker>
                        </b-field>

                        <b-checkbox>Remember me</b-checkbox>

                    </section>
                    <footer class="modal-card-foot">
                        <button class="button" type="button" @click="$parent.close()">Close</button>
                        <button class="button is-primary">Sign up!</button>
                    </footer>
                </div>
            </form>
</template>

<script>
export default{
  data() {
    return {
      firstname: '',
      lastname: '',
      email: '',
      birthdate: date,
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
body {
    text-align:left;
}
</style>
