<template>
  <div>
    <div id="spa_page0" v-if="show_content">
        <b-img src="~assets/IMG_7586_web.jpg" fluid></b-img>
    </div>
    <div style="background: #BEDEC7; padding-bottom: 5vh" v-if="show_content">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-col align-h="start" text-left>
            <b-row align-h="start" text-left>
              <h5 class="text-left">
                Dieses verrückte Jahr neigt sich dem Ende zu und wir planen motiviert und optimistisch schon 2021.
              </h5>
              <p class="text-left">
                Es sind einige schöne Projekte in den Startlöchern. Dabei sind wir aber ganz ehrlich:
                Wir wissen nicht was 2021 für uns bereit hält und was wir möglich machen können.
                Wir haben aber richtig Bock und werden unsere Pläne mit größter Flexibilität und Spontanität anpacken,
                realisieren und abfeiern. Wir freuen uns, wenn du dabei bist!
              </p>
              <p class="text-left">
                Wir haben hier aufgeschrieben, was schon klar ist und woran wir - solange es möglich ist -
                festhalten wollen. Das sind zum Beispiel Projektzeiträume oder Konzerttermine.
                Alles was fehlt, können wir euch einfach noch nicht sagen und das wird auch für uns erst klarer,
                wenn wir die konkrete Situation im Land kennen und einschätzen können. Manches ist hier kursiv
                geschrieben. Das sind beispielsweise Stücke, die wir 2020 schon vorhatten und die wir liebend gerne
                ins nächste Jahr verschieben würden. <strong>Ob das so passieren kann, wissen wir nicht und wir werden
                das möglicherweise noch anpassen müssen.</strong>
              </p>
              <pw class="text-left">
                Du siehst, das nächste Jahr wird ein großes Überraschungspaket. Aber das macht es ja umso spannender. :)
              </pw>

              <ul class="text-left">
                <li>Bewerbungsschluss: 01.08.2020</li>
                <li>Aufführungen: 28.02./01.03.2021</li>
                <li>Konzerthaus Berlin, großer Saal</li>
                <li>Endproben ab 18.02.2021 in Berlin, einzelne Proben zuvor in Absprache mit den SängerInnen</li>
                <li>Endprobenphase und Konzerte werden entschädigt</li>
                <li>Musikalische Leitung: Joseph Bastian, Dramaturgie/Regie: Marlene Schleicher</li>
              </ul>
            </b-row>
          </b-col>
        </b-container>
      </div>

    <div v-if="show_content">
        <b-img src="~assets/c_IMG_2159.jpg Sophia Hegewald.jpg" fluid></b-img>
    </div>

    <div style="background: #ed6b6f; padding-bottom: 5vh" v-if="show_content">
      <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
        <b-col align-h="start" text-left>
          <b-row align-h="start" text-left>
            <h1>Die Ausschreibung</h1>
          </b-row>
          <b-row>
            <h4 class="text-left">Wir suchen:<br/></h4>
            <p class="text-left">
              Zwei Sänger (Tenor und Bass) und eine Sängerin (Sopran), die dem großen Saal im Konzerthaus und den
              jeweiligen Partien des „Freischütz“ stimmlich gewachsen sind. Das Projekt überschreitet
              Gattungsgrenzen und spielt mit den Biographien der HauptakteurInnen Max, Agathe und Kaspar. So wird
              nach neuen Perspektiven auf die Inhalte von Webers „Freischütz“ gesucht. Dieses Vorhaben erfordert
              von den SängerInnen ein hohes Maß an Spielfreude, stimmlicher Flexibilität und den Mut auch mit
              gesprochenen Texten auf der Bühne zu wirken.
            </p>
            <h4 class="text-left">
              Ablauf der Bewerbung:<br/>
            </h4>
            <p class="text-left">
              <strong>Phase I: Digitale Bewerbung</strong> <br/>
              Wir wollen einen Eindruck von dir und deiner Stimme gewinnen und eine Vorstellung von deinem
              Blick auf die jeweilige Rolle bekommen. Auf Grundlage der Bewerbungen werden wir eine erste
              Auswahl treffen<br/><br/>

              <strong>Phase II: Workshop</strong> <br/>
              Für Phase II laden wir alle ausgewählten BewerberInnen gemeinsam zu einem eintägigen Bühnenworkshop
              Ende September in Berlin ein. Hierzu ist ebenfalls mindestens eine Arie aus dem „Freischütz“
              vorzubereiten, Details folgen mit der Einladung. Im Anschluss an den Workshop wird wiederum eine
              unabhängige Jury entscheiden, wer in “Hölle, Hölle, Hölle, Hölle!” mitspielen darf.
            </p>

          </b-row>
        </b-col>
      </b-container>
    </div>

    <div v-if="show_content">
        <b-img src="~assets/c_IMG_4864_ps.jpg Simon Klimaschka .jpg" fluid></b-img>
    </div>

    <b-overlay :show="show_overlay">
      <b-form @submit="onSubmit">
        <div style="background: #3DBAEC; padding-bottom: 5vh" v-if="show_content">
          <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
            <b-col align-h="start" text-left>
              <b-row align-h="start" text-left>
                <h1>Die Bewerbung</h1>
                <p class="text-left">Wir freuen uns sehr auf eure Einsendungen und falls es noch Fragen gibt, schreib
                  an <a href="mailto:freischuetz@junge-norddeutsche.de">freischuetz@junge-norddeutsche.de</a>!<br/><br/>
                </p>
                <b-container>
                  <b-row cols=1 cols-sm=1 cols-md=3 cols-lg=3 cols-xl=3>
                    <b-col>
                      <b-form-group id="inputg-vorname" label="Vorname: *" label-for="input-vorname">
                        <b-form-input
                          id="input-vorname"
                          v-model="form.vorname"
                          required
                          placeholder="Erika">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-nachname" label="Nachname: *" label-for="input-nachname">
                        <b-form-input
                          id="input-nachname"
                          v-model="form.nachname"
                          required
                          placeholder="Musterfrau">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-geschlecht" label="Geschlecht: *" label-for="input-geschlecht">
                        <b-form-select
                          id="input-geschlecht"
                          v-model="form.geschlecht"
                          :options="geschlechter"
                          required></b-form-select>
                      </b-form-group>
                    </b-col>

                    <b-col>
                      <b-form-group id="inputg-ausbildung" label="Ausbildung: *" label-for="input-ausbildung">
                        <b-form-select
                          id="input-ausbildung"
                          v-model="form.ausbildung"
                          :options="ausbildungen"
                          required></b-form-select>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-studienort" label="Studienort: *" label-for="input-studienort">
                        <b-form-input
                          id="input-studienort"
                          v-model="form.studienort"
                          required
                          placeholder="Musterstadt">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-hflehrerin" label="Hauptfachlehrer*in: *" label-for="input-hflehrerin">
                        <b-form-input
                          id="input-hflehrerin"
                          v-model="form.hflehrerin"
                          required
                          placeholder="Prof. Mustermann">
                        </b-form-input>
                      </b-form-group>
                    </b-col>

                    <b-col>
                      <b-form-group id="inputg-geburtsdatum" label="Geburtsdatum: *" label-for="input-geburtsdatum">
                        <b-form-input
                          id="input-geburtsdatum"
                          v-model="form.geburtsdatum"
                          required
                          placeholder="20-01-1990">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-email" label="E-Mail: *" label-for="input-email">
                        <b-form-input
                          id="input-email"
                          v-model="form.email"
                          type="email"
                          required
                          placeholder="mail@example.com">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-handynummer" label="Handynummer: *" label-for="input-handynummer">
                        <b-form-input
                          id="input-handynummer"
                          v-model="form.handynummer"
                          required
                          placeholder="+4915112345678">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                  </b-row>
                </b-container>

                <p>Zeige uns zwei Videos, die deine aktuellen sängerischen Fähigkeiten widerspiegeln. Eines der
                  Video sollte dich mit einer frei zu wählenden Arie von Max, Agathe oder Kaspar aus dem „Freischütz“
                  zeigen. Im zweiten Video sollst du dich mit einem Kunstlied deiner Wahl vorstellen.
                  Stelle uns hier einen Link (Wetransfer, Youtube, o.ä.) zu deinen Videos zur Verfügung:</p>

                <b-container>
                  <b-col>
                    <b-row>
                      <b-form-group id="inputg-link-video" label="Link Video: *" label-for="input-link-video">
                        <b-form-input
                          id="input-link-video"
                          v-model="form.linkvideo"
                          required
                          placeholder="https://">
                        </b-form-input>
                      </b-form-group>
                    </b-row>
                    <b-row>
                      <b-form-group id="inputg-link-video2" label="Link Video 2: (falls benötigt)" label-for="input-link-video2">
                        <b-form-input
                          id="input-link-video2"
                          v-model="form.linkvideo2"
                          placeholder="https://">
                        </b-form-input>
                      </b-form-group>
                    </b-row>
                  </b-col>
                </b-container>

                <p>Sprich einen deutschen Text, lyrisch oder poetisch, deiner Wahl ein (ca. 3 Min.).
                  Stelle uns hier einen Link zu deiner Audiodatei zur Verfügung:</p>

                <b-container>
                  <b-col>
                    <b-row>
                      <b-form-group id="inputg-link-audio" label="Link Audio: *" label-for="input-link-audio">
                        <b-form-input
                          id="input-link-audio"
                          v-model="form.linkaudio"
                          required
                          placeholder="https://">
                        </b-form-input>
                      </b-form-group>
                    </b-row>
                  </b-col>
                </b-container>
              </b-row>
            </b-col>
          </b-container>
        </div>

        <div v-if="show_content">
          <b-img src="~assets/c_IMG_0267.jpg" fluid></b-img>
        </div>

        <div style="background: #BEDEC7; padding-bottom: 5vh" v-if="show_content">
          <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
            <b-row align-h="start" text-left>
              <b-col align-h="start" text-left>
                <h1>Zu deiner Rolle</h1>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <b-form-group label="Auf welche Rolle bewirbst du dich? *">
                  <b-form-radio-group
                    id="input-rolle"
                    v-model="form.rolle"
                    :options="rollen"
                    name="input-rolle-name"
                    required
                  ></b-form-radio-group>
                </b-form-group>
              </b-col>
            </b-row>

            <!-- Agathe -->

            <b-row>
              <b-col>
                <div v-if="form.rolle === 'Agathe'" style="padding-bottom: 20px">
                  <p style="margin-bottom: 0">Warum möchtest du Agathe spielen? *</p>
                  <b-form-textarea
                    id="input-agate1"
                    v-model="form.agate1"
                    :state="form.agate1.length <= 250"
                    placeholder="Maximal 250 Zeichen."
                    rows="3">
                  </b-form-textarea>
                </div>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <div v-if="form.rolle === 'Agathe'" style="padding-bottom: 20px">
                  <p style="margin-bottom: 0">Versetze dich in Agathes Lage: Wie könnte sie Max in der Situation des
                    Probeschusses unterstützen
                    und warum entscheidet sie sich dafür/dagegen? *</p>
                  <b-form-textarea
                    id="input-agate2"
                    v-model="form.agate2"
                    :state="form.agate2.length <= 250"
                    placeholder="Maximal 250 Zeichen."
                    rows="3">
                  </b-form-textarea>
                </div>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <div v-if="form.rolle === 'Agathe'" style="padding-bottom: 20px">
                  <p style="margin-bottom: 0">Nenne ein Lied/eine Arie/einen Text, außerhalb des "Freischütz", der
                    ebenfalls zu
                    Agathes Charakter oder Situation passen könnte. *</p>
                  <b-form-textarea
                    id="input-agate3"
                    v-model="form.agate3"
                    placeholder=""
                    rows="3">
                  </b-form-textarea>
                </div>
              </b-col>
            </b-row>

            <!-- Max -->

            <b-row>
              <b-col>
                <div v-if="form.rolle === 'Max'" style="padding-bottom: 20px">
                  <p style="margin-bottom: 0">Warum möchtest du Max spielen? *</p>
                  <b-form-textarea
                    id="input-max1"
                    v-model="form.max1"
                    :state="form.max1.length <= 250"
                    placeholder="Maximal 250 Zeichen."
                    rows="3">
                  </b-form-textarea>
                </div>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <div v-if="form.rolle === 'Max'" style="padding-bottom: 20px">
                  <p style="margin-bottom: 0">Versetze dich in Max Lage und überlege dir Alternativen, wie du den
                    Probeschuss gewinnen könntest ohne auf die Freikugeln von Kaspar zurückgreifen zu müssen. *</p>
                  <b-form-textarea
                    id="input-max2"
                    v-model="form.max2"
                    :state="form.max2.length <= 250"
                    placeholder="Maximal 250 Zeichen."
                    rows="3">
                  </b-form-textarea>
                </div>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <div v-if="form.rolle === 'Max'" style="padding-bottom: 20px">
                  <p style="margin-bottom: 0">Nenne ein Lied/eine Arie/einen Text, außerhalb des "Freischütz", der
                    ebenfalls zu
                    Max Charakter oder Situation passen könnte. *</p>
                  <b-form-textarea
                    id="input-max3"
                    v-model="form.max3"
                    placeholder=""
                    rows="3">
                  </b-form-textarea>
                </div>
              </b-col>
            </b-row>

            <!-- Kaspar -->

            <b-row>
              <b-col>
                <div v-if="form.rolle === 'Kaspar'" style="padding-bottom: 20px">
                  <p style="margin-bottom: 0">Warum möchtest du Kaspar spielen? *</p>
                  <b-form-textarea
                    id="input-kaspar1"
                    v-model="form.kaspar1"
                    :state="form.kaspar1.length <= 250"
                    placeholder="Maximal 250 Zeichen."
                    rows="3">
                  </b-form-textarea>
                </div>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <div v-if="form.rolle === 'Kaspar'" style="padding-bottom: 20px">
                  <p style="margin-bottom: 0">Kaspar hat Max dazu überredet mit ihm in die Wolfsschlucht zu gehen.
                    Nun trifft er auf Agathe. Was hat er ihr zu sagen? *</p>
                  <b-form-textarea
                    id="input-kaspar2"
                    v-model="form.kaspar2"
                    :state="form.kaspar2.length <= 250"
                    placeholder="Maximal 250 Zeichen."
                    rows="3">
                  </b-form-textarea>
                </div>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <div v-if="form.rolle === 'Kaspar'" style="padding-bottom: 20px">
                  <p style="margin-bottom: 0">Nenne ein Lied/eine Arie/einen Text, außerhalb des "Freischütz", der
                    ebenfalls zu
                    Kaspars Charakter oder Situation passen könnte. *</p>
                  <b-form-textarea
                    id="input-kaspar3"
                    v-model="form.kaspar3"
                    placeholder=""
                    rows="3">
                  </b-form-textarea>
                </div>
              </b-col>
            </b-row>

            <b-row>
              <b-col>
                <p style="margin-bottom: 0">Als letztes noch dein tabellarischer Lebenslauf: *</p>
                <b-form-textarea
                  id="input-lebenslauf"
                  v-model="form.lebenslauf"
                  placeholder=""
                  rows="3"
                  required>
                </b-form-textarea>
              </b-col>
            </b-row>

          </b-container>
        </div>

        <div style="background: #FCE0D9" v-if="show_content">
          <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
            <b-row align-h="start" text-left>
              <b-col align-h="start" text-left>
                <h1>Absenden</h1>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <p>Alle Felder befüllt und die Fragen beantwortet? Eins fehlt noch:</p>
                <b-form-checkbox
                  id="input-datenschutz"
                  v-model="form.datenschutz"
                  name="input-datenschutz"
                  value="true"
                  unchecked-value="false"
                  required>
                  Ich stimme der Speicherung und Verarbeitung meiner Daten zu. *
                </b-form-checkbox>
              </b-col>
            </b-row>
            <b-row style="padding-top: 20px; padding-bottom: 1vh">
              <b-col>
                <b-button type="submit" variant="primary">Absenden</b-button>
              </b-col>
            </b-row>
            <b-row>
              <b-col v-if="show_error" style="">
                <h2 style="color: #ff4500">Es gab ein Problem beim Absenden des Formulars.</h2>
                <p class="danger">Wenn es beim erneuten Absenden wieder zu einem Problem kommt, schick eine Mail
                  an <a href="mailto:digital@junge-norddeutsche.de">digital@junge-norddeutsche.de</a> mit folgendem
                Inhalt:</p>
                <b-form-textarea
                  id="tmp"
                  v-model="form_as_json"
                  placeholder=""
                  rows="3"
                  max-rows="6"
                ></b-form-textarea>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <a href="https://junge-norddeutsche.de/impressum/">Impressum</a>
              </b-col>
            </b-row>
          </b-container>
        </div>
      </b-form>
    </b-overlay>

    <!-- After registration is finished -->
    <div style="background: #BEDEC7; height: 100vh" v-if="!show_content">
      <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
        <b-row align-h="start" text-left>
          <b-col align-h="start" text-left>
            <h1>Deine Bewerbung wurde versandt!</h1>
          </b-col>
        </b-row>
        <b-row>
          <b-col>
            <p>Du bekommst auch noch eine Bestätigungsmail mit den Informationen, die du im Formular angegeben hast.
            Noch Fragen? Melde dich unter
              <a href="mailto:freischuetz@junge-norddeutsche.de">freischuetz@junge-norddeutsche.de</a>!</p>
          </b-col>
        </b-row>
        <b-row>
          <b-col>
            <a href="https://junge-norddeutsche.de/impressum/">Impressum</a>
          </b-col>
        </b-row>
      </b-container>
    </div>
  </div>
</template>

<script>
import axios from '@nuxtjs/axios'

export default {
  data() {
    return {
      show_overlay: false,
      show_content: true,
      show_error: false,
      form: {
        vorname: '',
        nachname: '',
        geschlecht: '',
        ausbildung: '',
        studienort: '',
        hflehrerin: '',
        geburtsdatum: '',
        email: '',
        handynummer: '',
        rolle: '',
        linkvideo: '',
        linkvideo2: '',
        linkaudio: '',
        agate1: '',
        agate2: '',
        agate3: '',
        max1: '',
        max2: '',
        max3: '',
        kaspar1: '',
        kaspar2: '',
        kaspar3: '',
        lebenslauf: '',
        datenschutz: '',
      },
      form_as_json: "",
      geschlechter: ["weiblich", "männlich", "divers"],
      ausbildungen: ["BA Künstlerische Ausbildung", "MA Künstlerische Ausbildung",
        "BA Künstlerisch-pädagogische Ausbildung", "MA Künstlerisch-pädagogische Ausbildung", "Sonstiges"],
      rollen: ["Agathe", "Max", "Kaspar"]
    }
  },
  methods: {
    onSubmit(evt) {
      evt.preventDefault()
      this.show_overlay = true
      let error_occurred = false
      this.$axios.post('https://q890lmswhj.execute-api.us-east-2.amazonaws.com/default/hoelle_bewerbung/', JSON.stringify(this.form), {
          headers: {'Content-Type': 'application/json',
          'x-api-key': 'zDtjhmHfdRtQGF0b3AFx2KsQeuutxEL8mmFqp3k7'}
        })
        .then(response => {
          console.log(response);
          this.show_overlay = false
          this.show_content = false
        })
        .catch(e => {
          console.log(e);
          this.show_overlay = false
          this.show_content = true
          this.show_error = true
          this.form_as_json = JSON.stringify(this.form)
          this.form_as_json += " | "
          this.form_as_json += e
        })
        .finally(function () {
        });


    },

  }
}
</script>

<style>
p, li, ul {

  font-weight: 300;
  font-style: normal;
}
h1, h2, h3, h4, h5 {

  font-weight: 500;
  font-style: normal;
}
</style>
