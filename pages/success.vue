<template>
  <div>
    <div style="background-color: #000000">
      <b-container fluid class="align-items-baseline" style="padding-top: 1vh; padding-bottom: 1vh" align-h="start" text-left>
        <b-row>
          <b-col>
            <b-img style="height: 5vh" src="~assets/logo_jnp_2019_white_wo_text_trans.png"></b-img>
          </b-col>
        </b-row>
      </b-container>
    </div>

    <div style="background: #3DBAEC; padding-bottom: 5vh; height:93vh">
      <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
        <b-row>
          <b-col>
            <h1>
              Deine Bewerbung war erfolgreich!
            </h1>
            <p>
              Glückwunsch! Deine Bewerbung ist auf dem Weg zu uns und unser Besetzungsteam wird sich nach Ablauf der
              Bewerbungsfrist bei dir melden. Natürlich nicht direkt am nächsten Tag, aber immer rechtzeitig vor dem
              Projekt.
            </p>
            <p>
              Wenn du Fragen zur Bewerbung an sich hast, melde dich beim
              <a href="mailto:besetzung@junge-norddeutsche.de">Besetzungsteam</a>, wenn du eine technische Frage
              hast melde dich bei unserem <a href="mailto:digital@junge-norddeutsche.de">Digitalteam</a>.
            </p>
          </b-col>
        </b-row>
      </b-container>
    </div>
  </div>
</template>

<script>
export default {
name: "success.vue"
}
</script>

<style scoped>

</style>
