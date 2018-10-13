<template>
            <form action="">
                <div class="modal-card" style="width: 425px">
                    <header class="modal-card-head">
                        <p class="modal-card-title">Login</p>
                    </header>
                    <section class="modal-card-body">
                        <b-field label="Email">
                            <b-input
                                type="email"
                                :value="email"
                                placeholder="Your email"
                                required>
                            </b-input>
                        </b-field>

                        <b-field label="Password">
                            <b-input
                                type="password"
                                :value="password"
                                password-reveal
                                placeholder="Your password"
                                required>
                            </b-input>
                        </b-field>
                        <b-field label="Select a date">
                            <b-datepicker
                                placeholder="Click to select..."
                                icon="calendar-today">
                            </b-datepicker>
                        </b-field>

                        <b-checkbox>Remember me</b-checkbox>

                    </section>
                    <footer class="modal-card-foot">
                        <button class="button" type="button" @click="$parent.close()">Close</button>
                        <button class="button is-primary">Login</button>
                    </footer>
                </div>
            </form>
</template>

<script>
 
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
</style>
