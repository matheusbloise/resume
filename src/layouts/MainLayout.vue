<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="bg-dark text-white" height-hint="98" style="height: 15vh">
      <q-toolbar>
        <q-toolbar-title>
          <div class="row justify-end q-mt-md">
            <div class="col-md-2">
              <span class="text-weight-bold">Matheus Bloise</span>
            </div>
          </div>
          <div class="row justify-end">
            <div class="col-md-2">
              <span>Software Developer</span>
            </div>
          </div>
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-drawer show-if-above v-model="right" side="right" bordered>
      <div class="q-pa-lg bg-grey-2" style="height: 100%">
        <div class="row justify-center">
          <q-avatar size="160px" class="q-mb-sm">
            <img src="https://media-exp1.licdn.com/dms/image/C4D03AQH5gks7bRvljQ/profile-displayphoto-shrink_800_800/0/1599520901364?e=1619049600&v=beta&t=_3g84yIQRMJiVY9ZOM0WjHAgJwUA5W0WBjYii61ER7w">
          </q-avatar>
        </div>
        <span class="text-weight-bold">@matheusbloise</span>
        <div style="margin-top: 5px">
          <span class="text-weight-regular">Technical skills</span>
        </div>

        <div class="q-pt-md">
          <span>
            Development solutions with several technologies,
            see below some listed skills that i worked to solve real problems.
          </span>
        </div>
        <div class="row q-my-md justify-center">
          <div class="col-md-3">
            <q-img
              src="~assets/php.svg"
              style="width: 43px"
            />
          </div>
          <div class="col-md-8 q-mt-md">
            <q-linear-progress color="blue-9" size="10px" :value=0.9 />
          </div>
        </div>

        <div class="row q-my-md justify-center">
          <div class="col-md-3">
            <q-img
              src="~assets/js.svg"
              style="width: 46px"
            />
          </div>
          <div class="col-md-8 q-mt-md">
            <q-linear-progress color="blue-9" size="10px" :value=0.8 />
          </div>
        </div>

        <div class="row q-my-md justify-center">
          <div class="col-md-3">
            <q-img
              src="~assets/pgsql.svg"
              style="width: 42px"
            />
          </div>
          <div class="col-md-8 q-mt-md">
            <q-linear-progress color="blue-9" size="10px" :value=0.8 />
          </div>
        </div>
      </div>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  data () {
    return {
      right: false
    }
  }
}
</script>
