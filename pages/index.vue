<template>
  <div>
    <div style="background-color: #000000">
      <b-container fluid class="align-items-baseline" style="padding-top: 1vh; padding-bottom: 1vh" align-h="start" text-left>
        <b-row>
          <b-col>
            <a href="https://junge-norddeutsche.de">
              <b-img style="height: 5vh" src="~assets/logo_jnp_2019_white_wo_text_trans.png"></b-img>
            </a>
          </b-col>
        </b-row>
      </b-container>
    </div>

    <div style="background-color: #ed6b6f">
      <b-container fluid style="padding-top: 2vh; padding-bottom: 2vh">
        <b-row align-h="start">
          <b-col class="d-flex justify-content-center" sm="12" lg="3">
            <b-card
          title="Orchestermusiker:in"
          img-src="~assets/spalte_orchester.jpg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
        >
          <b-card-text>
            Große Werke, große Dirigenten, großartige Orchesterprojekte - hier kannst du dich als Orchestermusiker:in bewerben.
          </b-card-text>

          <b-button v-on:click="show_content = 'orchester'; " href="#orchester-id" variant="primary">Als Orchestermusiker:in bewerben</b-button>
        </b-card>
          </b-col>
          <b-col class="d-flex justify-content-center" sm="12" lg="3">
            <b-card
          title="1to1-Musiker:in"
          img-src="~assets/spalte_1to1.jpg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
        >
          <b-card-text>
            Eine Musiker:in, eine Zuhörer:in, eine besondere Begegnung zwischen zwei Menschen, bei der nur die
            Musik spricht. Wenn du das gerne erleben und bei den 1to1-Konzerten in Hamburg spielen
            würdest, kannst du dich hier bewerben.
          </b-card-text>

          <b-button v-on:click="show_content = '1to1'" href="#1to1-id" variant="primary">Als 1to1-Musiker:in bewerben</b-button>
        </b-card>
          </b-col>
          <b-col class="d-flex justify-content-center" sm="12" lg="3">
            <b-card
          title="Ensemble/Projekt"
          img-src="~assets/spalte_ensemble.jpg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
        >
          <b-card-text>
            Ihr seid ein Ensemble, das als Kammermusikgruppe gerne die jnp vertreten möchte? Dann stellt euch uns
            vor und wir melden uns bei euch, wenn wir den passenden Gig für euch haben.
          </b-card-text>

          <b-button v-on:click="show_content = 'ensemble'" href="#ensemble-id" variant="primary">Mit Ensemble/Projekt bewerben</b-button>
        </b-card>
          </b-col>
          <b-col class="d-flex justify-content-center" sm="12" lg="3">
            <b-card
          title="Helfer:in"
          img-src="~assets/spalte_helfer.jpg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
        >
          <b-card-text>
            Wenn du denkst, dass du und deine Fähigkeiten uns und unsere Projekte noch besser machen können,
            könntest oder du uns einfach mit deinen helfenden Händen unterstützen willst, kannst du dich hier bewerben.
          </b-card-text>

          <b-button v-on:click="show_content = 'helfer'" href="#helfer-id" variant="primary">Als Helfer:in bewerben</b-button>
        </b-card>
          </b-col>
        </b-row>
      </b-container>
    </div>

    <transition-group name="fade" mode="out-in">
      <div key="default1" style="background: #3DBAEC; padding-bottom: 5vh;" v-if="show_content === 'default'">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-row>
            <b-col>

              <b-skeleton v-b-tooltip.hover title="Warum das sich hier bewegt? Wir warten darauf, als was du dich bewerben willst ;)" animation="" width="60%"></b-skeleton>
              <p>Oben auf eine Bewerbungsart klicken - dann kommen hier unten auch mehr Informationen.</p>
              <b-skeleton v-b-tooltip.hover title="Warum das sich hier bewegt? Wir warten darauf, als was du dich bewerben willst ;)" animation="" width="60%"></b-skeleton>

            </b-col>
          </b-row>
        </b-container>
      </div>
    </transition-group>

    <!-- ########################### ORCHESTER ###########################################-->
    <transition-group name="fade" mode="out-in">
      <div id="orchester-id" key="orchester1" style="background: #BEDEC7; padding-bottom: 5vh" v-if="show_content === 'orchester'">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-row>
            <b-col>
              <h3 class="text-left">
                Moin und Servus!
              </h3>
              <h5 class="text-left">
                Schön dass du da bist!
              </h5>
              <p class="text-left">
                Dieses verrückte Jahr neigt sich dem Ende zu und wir planen motiviert und optimistisch schon 2021.
                Es stehen einige schöne Projekte in den Startlöchern. Dabei sind wir aber ganz ehrlich: Wir wissen
                nicht was 2021 für uns bereit hält. Was allerdings feststeht: Wir haben richtig Bock und
                werden unsere Pläne mit größter Flexibilität und Spontanität anpacken, realisieren und abfeiern.
                Wir freuen uns, wenn du dabei bist!
              </p>
              <p class="text-left">
                Wir haben hier aufgeschrieben, was schon klar ist und woran wir - solange es möglich ist - festhalten
                wollen. Das sind zum Beispiel Projektzeiträume oder Konzerttermine. Alles weitere können wir euch
                einfach noch nicht sagen und das wird auch für uns erst klarer, wenn wir die konkrete Situation im Land
                kennen und einschätzen können. Stücke, die wir 2020 schon vorhatten und die wir liebend gerne ins
                nächste Jahr verschieben würden, sind kursiv geschrieben. Ob das so passieren kann, wissen wir nicht
                und wir werden möglicherweise Programme und Besetzungen noch anpassen müssen.
              </p>
              <p class="text-left">
                Du siehst, das nächste Jahr wird ein großes Überraschungspaket. Aber das macht es ja umso spannender. :)
              </p>
            </b-col>
          </b-row>
        </b-container>
      </div>
      <div key="orchester2" style="background: #FCE0D9; padding-bottom: 5vh" v-if="show_content === 'orchester'">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-row>
            <b-col>
              <h3 class="text-left">
                Hölle, Hölle, Hölle, Hölle!
              </h3>
              <h5 class="text-left">
                18. Februar bis 1. März 2021
              </h5>
              <p class="text-left">
                Das Kammerspiel rund um Max, Agathe und Kaspar geht in die nächste Runde: Nach Aufnahme-Sessions
                im Hamburger Wald ziehen wir mit unserer Fassung des “Freischütz” kommenden Februar ins Konzerthaus Berlin.
                Ohne Orchestergraben bestreiten alle Instrumentalist:innen gemeinsam mit drei Sänger:innen den
                allgegenwärtigen Pakt mit dem Teufel und lassen neue Lesarten des romantischen Stoffes
                hör- und sichtbar werden.
              </p>
              <p class="text-left">
                <strong>Programm: </strong><a href="https://www.youtube.com/watch?v=FEGJxoywxDM">Der Freischütz - C.M Weber</a>
              </p>
              <p class="text-left">
                <strong>Dirigent: </strong> Joseph Bastian
              </p>
              <p class="text-left">
                <strong>Konzerte: </strong> 28. Februar und 1. März im Konzerthaus Berlin
              </p>
              <p class="text-left">
                <strong>Anmeldeschluss: 31. Januar 2021</strong>
              </p>
            </b-col>
          </b-row>
        </b-container>
      </div>

      <div key="orchester3" style="background: #ed6b6f; padding-bottom: 5vh" v-if="show_content === 'orchester'">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-row>
            <b-col>
              <h3 class="text-left">
                Himmelblau
              </h3>
              <h5 class="text-left">
                07. bis 15. April 2021, inkl. Workshop am 21./22. Februar 2021
              </h5>
              <p class="text-left">
                Unser Frühlingsprojekt, bunt wie ein Osterei: Sinfonie trifft Schauspiel, Beethoven trifft Eichendorff.
                Du hast 2020 noch nicht genug von Beethoven bekommen? Dann bist du hier genau richtig, wir machen
                nämlich einfach weiter. Und zwar mit Beethovens 6. Sinfonie, ‘nem richtig duften Klassiker. Wir
                freuen uns, dass mit Duncan Ward ein Rising Star des Dirigentenhimmels mit uns musizieren wird.
                Was hat das Ganze jetzt mit Schauspiel zu tun, fragt ihr euch? Wir bekommen Unterstützung von den
                coolen Typ:innen des Backstage Jugendclubs vom Schauspielhaus Hamburg. Sie haben ihre Inszenierung
                von Eichendorffs „Aus dem Leben eines Taugenichts“ im Gepäck. Und jetzt wird’s richtig bunt: Szenische
                Sequenzen wechseln sich mit Beethovens Musik ab und lassen ein schniekes Gesamtkunstwerk entstehen!
              </p>
              <p class="text-left">
                <strong>Programm: </strong><a href="https://www.youtube.com/watch?v=Zv4PIFRpYcw">Sinfonie Nr. 6 „Pastorale“ - L. Beethoven</a>
              </p>
              <p class="text-left">
                <strong>Dirigent: </strong>Duncan Ward
              </p>
              <p class="text-left">
                <strong>Konzerte: </strong>14. und 15. April in der Elbphilharmonie
              </p>
              <p class="text-left">
                <strong>Anmeldeschluss: 31. Januar 2021</strong>
              </p>
            </b-col>
          </b-row>
        </b-container>
      </div>

      <div key="orchester4" style="background: #BEDEC7; padding-bottom: 5vh" v-if="show_content === 'orchester'">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-row>
            <b-col>
              <h3 class="text-left">
                Trikestra
              </h3>
              <h5 class="text-left">
                19. bis 22. Mai 2021
              </h5>
              <p class="text-left">
                Trikestra - ein Projekt, das das DSO, das STEGREIF.orchester und die jnp vereint, geht in die
                letzte Runde. Es gab jedes Jahr Konzerte, die jeweils eins der drei Orchester geplant und die
                alle drei Orchester gemeinsam realisiert haben. In diesem Jahr ist das DSO unser Gastgeber und wir
                werden einige Musiker:innen nach Berlin schicken, um mit dem letzten Konzert diese 3-jährige Reihe
                zu beschließen.
              </p>
              <p class="text-left">
                <strong>Programm: </strong><a href="https://www.youtube.com/watch?v=Isic2Z2e2xs">Die Planeten - G. Holst</a>
              </p>
              <p class="text-left">
                <strong>Dirigent: </strong>Jonathan Bloxham
              </p>
              <p class="text-left">
                <strong>Konzerte: </strong>22. Mai 2021 im großen Sendesaal/Haus des Rundfunks Berlin
              </p>
              <p class="text-left">
                <strong>zusammen mit </strong>Mitgliedern des STEGREIF.orchesters, Mitglied des Deutschen Sinfonieorchesters Berlin (DSO)
              </p>
              <p class="text-left">
                <strong>Anmeldeschluss: 31. Januar 2021</strong>
              </p>
            </b-col>
          </b-row>
        </b-container>
      </div>

      <div key="orchester5" style="background: #3DBAEC; padding-bottom: 5vh" v-if="show_content === 'orchester'">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-row>
            <b-col>
              <h3 class="text-left">
                DETECT
              </h3>
              <h5 class="text-left">
                19. Juli bis 5. August 2021
              </h5>
              <p class="text-left">
                Unser jnp-Baby. Wir würden uns freuen, das große Sommerprojekt inklusive DETECT Festival mit euch zu
                feiern. Weil das aber ein sehr großes Vorhaben ist und es noch so weit in der Zukunft liegt, steht noch
                in den Sternen, wie das Ganze aussehen wird. Wir würden gerne die magische Miesmuschel fragen, ob wir
                ein normales Sommerprojekt haben können, ob wir nur ein kleines Orchester spielen lassen können oder ob
                wir mit 3 Orchestern an verschiedenen Standorten arbeiten werden, die dann zum Konzert zusammenkommen...
                Wir werden sehen und wir werden uns was Schönes für euch überlegen.
              </p>
              <p class="text-left">
                <strong>Programm: </strong>
              </p>
                <ul>
                  <li><a href="https://www.youtube.com/watch?v=uSIwiWA5c2U"><i>Konzert für Orchester - B. Bartok</i></a></li>
                  <li><a href="https://www.youtube.com/watch?v=OCUioWyKo1I"><i>Romeo und Julia - S. Prokofiev</i></a></li>
                  <li><a href="https://www.youtube.com/watch?v=vMcEbC4_1Tk"><i>La Valse -  M. Ravel</i></a></li>
                  <li><i>Konzerte für Saxophon Quartett, Akkordeon</i></li>
                </ul>
              <p class="text-left">
                <strong>Solisten: </strong>Signum Saxophon Quartett, Tamas Palfàlvi
              </p>
              <p class="text-left">
                <strong>Dirigent: </strong>Baldur Brönnimann
              </p>
              <p class="text-left">
                <strong>Konzerte: </strong>DETECT Festival vom 30. Juli bis 1. August, 4. und 5. August
              </p>
              <p class="text-left">
                <strong>Anmeldeschluss: 01. Mai 2021</strong>
              </p>
              <br/>
              <br/>
              <h5 class="text-left">
                <strong>Änderungen bei allen Projekten vorbehalten.</strong>
              </h5>
            </b-col>
          </b-row>
        </b-container>
      </div>

      <div key="orchester6" style="background: #BEDEC7; padding-bottom: 5vh" v-if="show_content === 'orchester'">
        <b-form @submit="onSubmitOrchester">
          <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
            <b-row align-h="start" text-left>
              <b-col cols="12" align-h="start" text-left>
                Überzeugt? Dann benötigen wir nur noch ein paar Informationen von dir!
              </b-col>
              <b-col cols="12" align-h="start" text-left>
                <b-container>
                  <b-row cols=1 cols-sm=1 cols-md=3 cols-lg=3 cols-xl=3>
                    <b-col>
                      <b-form-group id="inputg-orchester-vorname" label="Vorname: *" label-for="input-orchester-vorname">
                        <b-form-input
                          id="input-orchester-vorname"
                          v-model="form_orchester.vorname"
                          required
                          placeholder="Erika">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-orchester-nachname" label="Nachname: *" label-for="input-orchester-nachname">
                        <b-form-input
                          id="input-orchester-nachname"
                          v-model="form_orchester.nachname"
                          required
                          placeholder="Musterfrau">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-orchester-geschlecht" label="Geschlecht: *" label-for="input-orchester-geschlecht">
                        <b-form-select
                          id="input-orchester-geschlecht"
                          v-model="form_orchester.geschlecht"
                          :options="geschlechter"
                          required></b-form-select>
                      </b-form-group>
                    </b-col>

                    <b-col>
                      <b-form-group id="inputg-orchester-ausbildung" label="Ausbildung: *" label-for="input-orchester-ausbildung">
                        <b-form-select
                          id="input-orchester-ausbildung"
                          v-model="form_orchester.ausbildung"
                          :options="ausbildungen"
                          required></b-form-select>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-orchester-instrument" label="Instrument: *" label-for="input-orchester-instrument">
                        <b-form-input
                          id="input-orchester-instrument"
                          v-model="form_orchester.instrument"
                          required
                          placeholder="Klarinette">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-orchester-studienort" label="Studienort: *" label-for="input-orchester-studienort">
                        <b-form-input
                          id="input-orchester-studienort"
                          v-model="form_orchester.studienort"
                          required
                          placeholder="Musterstadt">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-orchester-hflehrerin" label="Hauptfachlehrer:in: *" label-for="input-orchester-hflehrerin">
                        <b-form-input
                          id="input-orchester-hflehrerin"
                          v-model="form_orchester.hflehrerin"
                          required
                          placeholder="Prof. Musterfrau">
                        </b-form-input>
                      </b-form-group>
                    </b-col>

                    <b-col>
                      <b-form-group id="inputg-orchester-geburtsdatum" label="Geburtsdatum: *" label-for="input-orchester-geburtsdatum">
                        <b-form-input
                          id="input-orchester-geburtsdatum"
                          v-model="form_orchester.geburtsdatum"
                          required
                          placeholder="20-01-1990">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-orchester-email" label="E-Mail: *" label-for="input-orchester-email">
                        <b-form-input
                          id="input-orchester-email"
                          v-model="form_orchester.email"
                          type="email"
                          required
                          placeholder="mail@example.com">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-orchester-handynummer" label="Handynummer: *" label-for="input-orchester-handynummer">
                        <b-form-input
                          id="input-orchester-handynummer"
                          v-model="form_orchester.handynummer"
                          required
                          placeholder="+49 123 4567890">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                  </b-row>
                </b-container>
              </b-col>
            </b-row>
            <b-row>
              <b-col cols="12">
                <b-form-group label="Für welche Projekte willst du dich bewerben?">
                  <b-form-checkbox
                    v-for="option in optionen_projekte"
                    v-model="form_orchester.projekte"
                    :key="option.value"
                    :value="option.value"
                    name="flavour-3a"
                  >
                    {{ option.text }}
                  </b-form-checkbox>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-orchester-werdegang" label="Dein (wesentlicher) musikalischer Werdegang: *" label-for="input-orchester-werdegang">
                  <b-form-textarea
                    id="input-orchester-werdegang"
                    v-model="form_orchester.werdegang"
                    required
                    placeholder="Ungefähr 100 bis 200 Wörter.">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-orchester-erfahrungen" label="Was sind Deine wichtigsten Orchestererfahrungen? Welche Werke wurden dabei in den genannten Orchestern gespielt? Kurze Stichpunkte! *" label-for="input-orchester-erfahrungen">
                  <b-form-textarea
                    id="input-orchester-erfahrungen"
                    v-model="form_orchester.erfahrungen"
                    required
                    placeholder="Ungefähr 100 bis 200 Wörter.">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-orchester-reizt" label="Erzähle uns noch, wie Du von der jnp erfahren hast und was Dich an unserem Projekt reizt: *" label-for="input-orchester-reizt">
                  <b-form-textarea
                    id="input-orchester-reizt"
                    v-model="form_orchester.reizt"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-orchester-beitragen" label="Was möchtest Du zum Gelingen der Projekte gerne beitragen? *" label-for="input-orchester-beitragen">
                  <b-form-textarea
                    id="input-orchester-beitragen"
                    v-model="form_orchester.beitragen"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-orchester-datenschutz" label="" label-for="input-orchester-datenschutz">
                  <b-form-checkbox
                    id="input-orchester-datenschutz"
                    v-model="form_orchester.datenschutz"
                    name="input-orchester-datenschutz"
                    value="true"
                    unchecked-value="false"
                    required>
                    Ich stimme der Speicherung und Verarbeitung meiner Daten zu. *
                  </b-form-checkbox>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-button id="orchester-submit-button" type="submit" variant="primary">Absenden</b-button>
              </b-col>
            </b-row>
          </b-container>
        </b-form>
      </div>

    </transition-group>
    <!-- ########################### 1TO1 ###########################################-->

    <transition-group name="fade" mode="out-in">
      <div id="1to1-id" key="1to11" style="background: #FCE0D9; padding-bottom: 5vh" v-if="show_content === '1to1'">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-row>
            <b-col>
              <h3 class="text-left">
                Moin und Servus!
              </h3>
              <h5 class="text-left">
                Schön dass du da bist!
              </h5>
              <p class="text-left">
                1 Musiker:in, 1 Hörer:in, 2 Meter Abstand - die 1:1 CONCERTS ermöglichen live-Konzerte im
                coronatauglichen Kleinstformat. Und das Ganze auch noch für einen guten Zweck, nämlich zur
                Unterstützung des Nothilfefonds der Deutschen Orchesterstiftung! Das Konzept sorgt gerade für
                viel Wirbel und hat es sogar
                <a href="https://www.nytimes.com/2020/06/05/world/europe/germany-stuttgart-coronavirus-reopening.html?fbclid=IwAR03dp5RCjQMFVl9QZxhRPqnrvOViOwDrgUlEm5-S7SbJSSz3O1Hm9EjZZI">
                  bis in die New York Times geschafft
                </a> hat. Auch wir sind seit einigen Monaten dabei und suchen nun nach Musiker:innen
                für unseren Standort Hamburg!
              </p>
              <p class="text-left">
                Ein Konzert besteht aus der Begegnung zweier Menschen (dir, als Musiker:in und dem/der Hörer:in).
                Diese Begegnung beinhaltet zuerst einen etwa einminütigen Augenkontakt und dann 10 Minuten Musik,
                die du deinem Gast solistisch vorspielen willst. Dabei kannst du spontan entscheiden, was zu deinem
                Gegenüber passt und was du vortragen willst. Wenn du aus dem Raum Hamburg kommst, oder bereit bist,
                mal nach Hamburg zu fahren und Bock auf so ein intimes und emotionales Konzerterlebnis hast,
                freuen wir uns, wenn du dich bei uns bewirbst. Wenn du vorher aber noch ein bisschen mehr Infos haben
                möchtest oder du dir schon wichtige Fragen stellst, kannst du
                <a href="https://junge-norddeutsche.de/1to1/">hier</a> einiges nachlesen oder dem
                <a href="mailto:1to1concerts@junge-norddeutsche.de">1to1 Team</a> anrufen.
              </p>
            </b-col>
          </b-row>
        </b-container>
      </div>

      <div key="1to12" style="background: #BEDEC7; padding-bottom: 5vh" v-if="show_content === '1to1'">
        <b-form @submit="onSubmit1to1">
          <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
            <b-row align-h="start" text-left>
              <b-col cols="12" align-h="start" text-left>
                Überzeugt? Dann benötigen wir nur noch ein paar Informationen von dir!
              </b-col>
              <b-col cols="12" align-h="start" text-left>
                <b-container>
                  <b-row cols=1 cols-sm=1 cols-md=3 cols-lg=3 cols-xl=3>
                    <b-col>
                      <b-form-group id="inputg-1to1-vorname" label="Vorname: *" label-for="input-1to1-vorname">
                        <b-form-input
                          id="input-1to1-vorname"
                          v-model="form_1to1.vorname"
                          required
                          placeholder="Erika">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-1to1-nachname" label="Nachname: *" label-for="input-1to1-nachname">
                        <b-form-input
                          id="input-1to1-nachname"
                          v-model="form_1to1.nachname"
                          required
                          placeholder="Musterfrau">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-1to1-geschlecht" label="Geschlecht: *" label-for="input-1to1-geschlecht">
                        <b-form-select
                          id="input-1to1-geschlecht"
                          v-model="form_1to1.geschlecht"
                          :options="geschlechter"
                          required></b-form-select>
                      </b-form-group>
                    </b-col>

                    <b-col>
                      <b-form-group id="inputg-1to1-ausbildung" label="Ausbildung: *" label-for="input-1to1-ausbildung">
                        <b-form-select
                          id="input-1to1-ausbildung"
                          v-model="form_1to1.ausbildung"
                          :options="ausbildungen"
                          required></b-form-select>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-1to1-studienort" label="Studienort: *" label-for="input-1to1-studienort">
                        <b-form-input
                          id="input-1to1-studienort"
                          v-model="form_1to1.studienort"
                          required
                          placeholder="Musterstadt">
                        </b-form-input>
                      </b-form-group>
                    </b-col>

                    <b-col>
                      <b-form-group id="inputg-1to1-geburtsdatum" label="Geburtsdatum: *" label-for="input-1to1-geburtsdatum">
                        <b-form-input
                          id="input-1to1-geburtsdatum"
                          v-model="form_1to1.geburtsdatum"
                          required
                          placeholder="20-01-1990">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-1to1-email" label="E-Mail: *" label-for="input-1to1-email">
                        <b-form-input
                          id="input-1to1-email"
                          v-model="form_1to1.email"
                          type="email"
                          required
                          placeholder="mail@example.com">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-1to1-handynummer" label="Handynummer: *" label-for="input-1to1-handynummer">
                        <b-form-input
                          id="input-1to1-handynummer"
                          v-model="form_1to1.handynummer"
                          required
                          placeholder="+49 123 4567890">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                  </b-row>
                </b-container>
              </b-col>
            </b-row>
            <b-row>
              <b-col cols="12">
                <b-form-group id="inputg-1to1-werdegang" label="Dein (wesentlicher) musikalischer Werdegang und deine Konzerterfahrungen: *" label-for="input-1to1-werdegang">
                  <b-form-textarea
                    id="input-1to1-werdegang"
                    v-model="form_1to1.werdegang"
                    required
                    placeholder="Ungefähr 100 bis 200 Wörter.">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-1to1-erhoffen" label="Was erhoffst du dir von den Begegnungen bei den 1to1 Konzerten? *" label-for="input-1to1-erhoffen">
                  <b-form-textarea
                    id="input-1to1-erhoffen"
                    v-model="form_1to1.erhoffen"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-1to1-datenschutz" label="" label-for="input-1to1-datenschutz">
                  <b-form-checkbox
                    id="input-1to1-datenschutz"
                    v-model="form_1to1.datenschutz"
                    name="input-1to1-datenschutz"
                    value="true"
                    unchecked-value="false"
                    required>
                    Ich stimme der Speicherung und Verarbeitung meiner Daten zu. *
                  </b-form-checkbox>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-button id="1to1-submit-button" type="submit" variant="primary">Absenden</b-button>
              </b-col>
            </b-row>
          </b-container>
        </b-form>
      </div>
    </transition-group>
    <!-- ########################### ENSEMBLE ###########################################-->

    <transition-group name="fade" mode="out-in">
      <div id="ensemble-id" key="ensemble1" style="background: #3DBAEC; padding-bottom: 5vh" v-if="show_content === 'ensemble'">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-row>
            <b-col>
              <h3 class="text-left">
                Moin und Servus!
              </h3>
              <h5 class="text-left">
                Schön dass ihr da seid!
              </h5>
              <p class="text-left">
                Es soll schon vorgekommen sein, dass wir die ein oder andere Preisverleihung oder die Eröffnung einer
                neuen Konzertkirche umrahmen sollten. Und immer wieder mussten wir uns überlegen, wer, mit welchem
                Ensemble, das dann vielleicht sogar spontan zusammengewürfelt werden muss, spielen kann. Aber
                eigentlich sind wir uns sicher, dass es im großen jnp-Land einige Ensembles, Formationen oder
                Gruppen gibt, die gerne für uns unterwegs sind und die ein oder andere zusätzliche Konzertmöglichkeit
                wahrnehmen wollen. Gerade nächstes Jahr, wo noch nicht einzuschätzen ist, wie viele Leute wir auf
                die Bühnen stellen und setzen können, wäre es großartig aus einem Pool an Gruppen schöpfen zu
                können. Wir freuen uns über die Bewerbung von dir und deinen Kolleg:innen.
              </p>
            </b-col>
          </b-row>
        </b-container>
      </div>

      <div key="ensemble2" style="background: #BEDEC7; padding-bottom: 5vh" v-if="show_content === 'ensemble'">
        <b-form @submit="onSubmitEnsemble">
          <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
            <b-row align-h="start" text-left>
              <b-col cols="12" align-h="start" text-left>
                Überzeugt? Dann benötigen wir nur noch ein paar Informationen von euch!
              </b-col>
              <b-col cols="12" align-h="start" text-left>
                <b-container>
                  <b-row cols=1 cols-sm=1 cols-md=3 cols-lg=3 cols-xl=3>
                    <b-col>
                      <b-form-group id="inputg-ensemble-name" label="Name: *" label-for="input-ensemble-name">
                        <b-form-input
                          id="input-ensemble-name"
                          v-model="form_ensemble.name"
                          required
                          placeholder="Erika Musterfrau">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-ensemble-ensemblename" label="Ensemblename: *" label-for="input-ensemble-ensemblename">
                        <b-form-input
                          id="input-ensemble-ensemblename"
                          v-model="form_ensemble.ensemblename"
                          required
                          placeholder="Musterquartriotett">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-ensemble-standort" label="Standort: *" label-for="input-ensemble-standort">
                        <b-form-input
                          id="input-ensemble-standort"
                          v-model="form_ensemble.standort"
                          required
                          placeholder="Musterstadt">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-ensemble-email" label="E-Mail: *" label-for="input-ensemble-email">
                        <b-form-input
                          id="input-ensemble-email"
                          v-model="form_ensemble.email"
                          type="email"
                          required
                          placeholder="mail@example.com">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-ensemble-handynummer" label="Handynummer: *" label-for="input-ensemble-handynummer">
                        <b-form-input
                          id="input-ensemble-handynummer"
                          v-model="form_ensemble.handynummer"
                          required
                          placeholder="+49 123 4567890">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                  </b-row>
                </b-container>
              </b-col>
            </b-row>
            <b-row>
              <b-col cols="12">
                <b-form-group id="inputg-ensemble-hardfacts" label="Hardfacts zu eurem Ensemble (Besetzung, Namen der Mitwirkenden, Repertoire, wie lange gibt es euch schon): *" label-for="input-ensemble-hardfacts">
                  <b-form-textarea
                    id="input-ensemble-hardfacts"
                    v-model="form_ensemble.hardfacts"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-ensemble-bezug" label="Was ist euer Bezug zur jnp? *" label-for="input-ensemble-bezug">
                  <b-form-textarea
                    id="input-ensemble-bezug"
                    v-model="form_ensemble.bezug"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-ensemble-reizt" label="Erzähle uns noch, wie Du von der jnp erfahren hast und was Dich an unserem Projekt reizt: *" label-for="input-ensemble-reizt">
                  <b-form-textarea
                    id="input-ensemble-reizt"
                    v-model="form_ensemble.reizt"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-ensemble-ausmachen" label="Was macht euch als Gruppe aus? Was wollt ihr mit euren Auftritten transportieren? *" label-for="input-ensemble-ausmachen">
                  <b-form-textarea
                    id="input-ensemble-ausmachen"
                    v-model="form_ensemble.ausmachen"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-ensemble-konzerterfahrungen" label="Schreibe kurz eure Konzerterfahrungen: *" label-for="input-ensemble-konzerterfahrungen">
                  <b-form-textarea
                    id="input-ensemble-konzerterfahrungen"
                    v-model="form_ensemble.konzerterfahrungen"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-ensemble-datenschutz" label="" label-for="input-ensemble-datenschutz">
                  <b-form-checkbox
                    id="input-ensemble-datenschutz"
                    v-model="form_ensemble.datenschutz"
                    name="input-ensemble-datenschutz"
                    value="true"
                    unchecked-value="false"
                    required>
                    Ich stimme der Speicherung und Verarbeitung meiner Daten zu. *
                  </b-form-checkbox>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-button id="ensemble-submit-button" type="submit" variant="primary">Absenden</b-button>
              </b-col>
            </b-row>
          </b-container>
        </b-form>
      </div>
    </transition-group>

    <!-- ########################### HELFER ###########################################-->

    <transition-group name="fade" mode="out-in">
      <div id="helfer-id" key="helfer1" style="background: #3DBAEC; padding-bottom: 5vh" v-if="show_content === 'helfer'">
        <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
          <b-row>
            <b-col>
              <h3 class="text-left">
                Moin und Servus!
              </h3>
              <h5 class="text-left">
                Schön dass du da bist!
              </h5>
              <p class="text-left">
                Wer glaubt, dass die jnp nur aus Musiker:innen besteht, die sich auf die Bühne setzen und ihr
                Konzert spielen, irrt ganz gewaltig. Denn da gibt es noch so einige Menschen im Hintergrund, die
                vor, während, und auch nach dem Projekt ackern, um das Ganze zu dem zu machen, was es ist.
                Im Grunde können wir nie genug von diesen Leuten haben, die Bock auf die jnp und alles rund um die
                Musik haben und deswegen sind wir immer auf der Suche nach Transporterfahrer:innen, Köch:innen,
                Fotograf:innen, Yogalehrer:innen, Physiotherapeut:innen, Psychotherapeut:innen, Springer:innen
                oder als was auch immer du dich bezeichnen magst! Vielleicht wissen wir ja noch gar nicht, dass wir
                dich und deine Fähigkeiten gebrauchen könnten und deshalb freuen wir uns, wenn du uns hier schreibst,
                was du kannst und womit du dich gerne einbringen wollen würdest.
              </p>
            </b-col>
          </b-row>
        </b-container>
      </div>

      <div key="helfer2" style="background: #BEDEC7; padding-bottom: 5vh" v-if="show_content === 'helfer'">
        <b-form @submit="onSubmitHelfer">
          <b-container class="align-items-baseline" style="padding-top: 5vh" align-h="start" text-left>
            <b-row align-h="start" text-left>
              <b-col cols="12" align-h="start" text-left>
                Überzeugt? Dann benötigen wir nur noch ein paar Informationen von dir!
              </b-col>
              <b-col cols="12" align-h="start" text-left>
                <b-container>
                  <b-row cols=1 cols-sm=1 cols-md=3 cols-lg=3 cols-xl=3>
                    <b-col>
                      <b-form-group id="inputg-helfer-vorname" label="Vorname: *" label-for="input-helfer-vorname">
                        <b-form-input
                          id="input-helfer-vorname"
                          v-model="form_helfer.vorname"
                          required
                          placeholder="Erika">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-helfer-nachname" label="Nachname: *" label-for="input-helfer-nachname">
                        <b-form-input
                          id="input-helfer-nachname"
                          v-model="form_helfer.nachname"
                          required
                          placeholder="Erika">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-helfer-email" label="E-Mail: *" label-for="input-helfer-email">
                        <b-form-input
                          id="input-helfer-email"
                          v-model="form_helfer.email"
                          type="email"
                          required
                          placeholder="mail@example.com">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="inputg-helfer-handynummer" label="Handynummer: *" label-for="input-helfer-handynummer">
                        <b-form-input
                          id="input-helfer-handynummer"
                          v-model="form_helfer.handynummer"
                          required
                          placeholder="+49 123 4567890">
                        </b-form-input>
                      </b-form-group>
                    </b-col>
                  </b-row>
                </b-container>
              </b-col>
            </b-row>
            <b-row>
              <b-col cols="12">
                <b-form-group label="Bei welchen Projekten hättest du Zeit?">
                  <b-form-checkbox
                    v-for="option in optionen_projekte"
                    v-model="form_helfer.projekte"
                    :key="option.value"
                    :value="option.value"
                    name="flavour-3a"
                  >
                    {{ option.text }}
                  </b-form-checkbox>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-helfer-uebernehmen" label="Welche Aufgaben könntest du übernehmen? Womit kannst du unsere Projekte bereichern? *" label-for="input-helfer-uebernehmen">
                  <b-form-textarea
                    id="input-helfer-uebernehmen"
                    v-model="form_helfer.uebernehmen"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-helfer-brennt" label="Was mir noch auf der Seele brennt: *" label-for="input-helfer-brennt">
                  <b-form-textarea
                    id="input-helfer-brennt"
                    v-model="form_helfer.brennt"
                    required
                    placeholder="">
                  </b-form-textarea>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-form-group id="inputg-helfer-datenschutz" label="" label-for="input-helfer-datenschutz">
                  <b-form-checkbox
                    id="input-helfer-datenschutz"
                    v-model="form_helfer.datenschutz"
                    name="input-helfer-datenschutz"
                    value="true"
                    unchecked-value="false"
                    required>
                    Ich stimme der Speicherung und Verarbeitung meiner Daten zu. *
                  </b-form-checkbox>
                </b-form-group>
              </b-col>
              <b-col cols="12">
                <b-button id="helfer-submit-button" type="submit" variant="primary">Absenden</b-button>
              </b-col>
            </b-row>
          </b-container>
        </b-form>
      </div>

    </transition-group>

    <div style="background-color: #000000">
      <b-container fluid class="align-items-baseline" style="padding-top: 1vh; padding-bottom: 1vh" align-h="start" text-left>
        <b-row>
          <b-col>
            <a href="https://junge-norddeutsche.de/impressum/">Impressum</a>
          </b-col>
        </b-row>
      </b-container>
    </div>

    <b-modal id="error-modal" v-model="show_error_modal">
      <h1>Sorry!</h1>
      <p>Es gab einen Fehler beim Abschicken deiner Bewerbung. Das kann an deiner Internetverbindung, allerdings auch an uns liegen.</p>
      <p>Am besten klickst du diese Meldung weg und probierst nochmals, deine Bewerbung abzuschicken.</p>
      <br/>
      <p>Du bist schon zum zweiten Mal hier? Sorry für die Unannehmlichkeiten! Kopier den folgenden Text und schick
        den Text an <a href="mailto:digital@junge-norddeutsche.de">digital@junge-norddeutsche.de</a>.</p>

      <b-form-textarea
                  id="tmp"
                  v-model="json_error_text"
                  placeholder=""
                  rows="3"
                  max-rows="6"
      ></b-form-textarea>

    </b-modal>

  </div>
</template>

<script>
import axios from '@nuxtjs/axios'

export default {
  data() {
    return {
      show_content: "default",
      json_error_text: "",
      show_error_modal: false,
      form_orchester: {
        identifier: 'orchester',
        vorname: '',
        nachname: '',
        geschlecht: '',
        ausbildung: '',
        studienort: '',
        hflehrerin: '',
        geburtsdatum: '',
        email: '',
        handynummer: '',
        lebenslauf: '',
        datenschutz: '',
        werdegang: '',
        beitragen: '',
        reizt: '',
        erfahrungen: '',
        projekte: [],
      },
      form_1to1: {
        identifier: '1to1',
        vorname: '',
        nachname: '',
        geschlecht: '',
        ausbildung: '',
        studienort: '',
        geburtsdatum: '',
        email: '',
        handynummer: '',
        datenschutz: '',
        werdegang: '',
        erhoffen: ''
      },
      form_ensemble: {
        identifier: 'ensemble',
        name: '',
        ensemblename: '',
        standort: '',
        email: '',
        handynummer: '',
        hardfacts: '',
        datenschutz: '',
        bezug: '',
        reizt: '',
        ausmachen: '',
        konzerterfahrungen: '',
      },
      form_helfer: {
        identifier: 'helfer',
        vorname: '',
        nachname: '',
        email: '',
        handynummer: '',
        datenschutz: '',
        uebernehmen: '',
        brennt: '',
        projekte: [],
      },
      geschlechter: ["weiblich", "männlich", "divers", "keine Angabe"],
      ausbildungen: ["BA Künstlerische Ausbildung", "MA Künstlerische Ausbildung",
        "BA Künstlerisch-pädagogische Ausbildung", "MA Künstlerisch-pädagogische Ausbildung", "Sonstiges"],
      optionen_projekte: [
          { text: 'Hölle, Hölle, Hölle, Hölle! (18.02 - 01.03)', value: 'hoelle' },
          { text: 'Himmelblau (07.04 - 15.04)', value: 'himmelblau' },
          { text: 'Trikestra (19.05 - 22.05)', value: 'trikestra' },
          { text: 'Detect (19.07 - 05.08)', value: 'detect' }
        ]
    }
  },
  methods: {
    onSubmitOrchester(evt) {
      evt.preventDefault()
      document.getElementById('orchester-submit-button').classList.add("disabled")
      this.$axios.post('https://bewerbung-service-run-rvzfazc5ja-ey.a.run.app', JSON.stringify(this.form_orchester), {
          headers: {'Content-Type': 'application/json'}
        })
        .then(response => {
          this.$router.push("/success")
          document.getElementById('orchester-submit-button').classList.remove("disabled")
        })
        .catch(e => {
          console.log(e);
          document.getElementById('orchester-submit-button').classList.remove("disabled")
          this.json_error_text = JSON.stringify(this.form_orchester)
          this.show_error_modal = true
        })
        .finally(function () {
        });
    },
    onSubmit1to1(evt) {
      evt.preventDefault()
      document.getElementById('1to1-submit-button').classList.add("disabled")
      this.$axios.post('https://bewerbung-service-run-rvzfazc5ja-ey.a.run.app', JSON.stringify(this.form_1to1), {
          headers: {'Content-Type': 'application/json'}
        })
        .then(response => {
          this.$router.push("/success")
          document.getElementById('1to1-submit-button').classList.remove("disabled")
        })
        .catch(e => {
          console.log(e);
          document.getElementById('1to1-submit-button').classList.remove("disabled")
          this.json_error_text = JSON.stringify(this.form_1to1)
          this.show_error_modal = true
        })
        .finally(function () {
        });
    },
    onSubmitEnsemble(evt) {
      evt.preventDefault()
      document.getElementById('ensemble-submit-button').classList.add("disabled")
      this.show_overlay = true
      this.$axios.post('https://bewerbung-service-run-rvzfazc5ja-ey.a.run.app', JSON.stringify(this.form_ensemble), {
          headers: {'Content-Type': 'application/json'}
        })
        .then(response => {
          this.$router.push("/success")
          document.getElementById('ensemble-submit-button').classList.remove("disabled")
        })
        .catch(e => {
          console.log(e);
          document.getElementById('ensemble-submit-button').classList.remove("disabled")
          this.json_error_text = JSON.stringify(this.form_ensemble)
          this.show_error_modal = true
        })
        .finally(function () {
        });
    },
    onSubmitHelfer(evt) {
      evt.preventDefault()
      document.getElementById('helfer-submit-button').classList.add("disabled")
      this.show_overlay = true
      this.$axios.post('https://bewerbung-service-run-rvzfazc5ja-ey.a.run.app', JSON.stringify(this.form_helfer), {
          headers: {'Content-Type': 'application/json'}
        })
        .then(response => {
          this.$router.push("/success")
          document.getElementById('helfer-submit-button').classList.remove("disabled")
        })
        .catch(e => {
          console.log(e);
          document.getElementById('helfer-submit-button').classList.remove("disabled")
          this.json_error_text = JSON.stringify(this.form_helfer)
          this.show_error_modal = true
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
.fade-enter-active, .fade-leave-active {
  transition: opacity .5s;
}
.fade-enter, .fade-leave-to {
  opacity: 0
}
</style>
