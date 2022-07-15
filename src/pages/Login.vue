<template>

    <div class="row" style="height: 90vh;">
      <div class="col-0 col-md-6 flex justify-center content-center">
        <img src="login.svg" class="responsive">
      </div>
      <div v-bind:class="{'justify-center': $q.screen.md || $q.screen.sm || $q.screen.xs }"
        class="col-12 col-md-6 flex content-center">

        <q-card v-bind:style="$q.screen.lt.sm ? {'width': '80%'} : {'width': '50%'}">
          <q-card-section>
            <q-avatar size="109px" class="absolute-center shadow-10">
              <img src="https://github.com/fernandogomesfg.png" alt="avatar">
            </q-avatar>
          </q-card-section>

          <q-card-section>
            <div class="q-pt-lg">
              <div class="col text-h6 ellipsis flex justify-center">
                <h2 class="text-h2 text-uppercase q-my-none text-weight-regular">
                  Login
                </h2>
              </div>
            </div>
          </q-card-section>

          <q-card-section>
            <q-form class="q-gutter-md">
              <q-input label="Username"> </q-input>
              <q-input label="Password" type="password"></q-input>

              <q-btn class="full-width"  color="primary" label="Login" rounded></q-btn>
              <q-btn class="full-width" label="Esqueceu senha?"  flat></q-btn>
              <q-btn class="full-width" label="Registrar" flat></q-btn>
            </q-form>
          </q-card-section>

        </q-card>
      </div>
    </div>



</template>

<script>


export default {
  name: 'LoginPage'
}
</script>
