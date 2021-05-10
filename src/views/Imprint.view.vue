<script lang="ts">
    import { Component, Vue } from "vue-property-decorator";

    import SvgIcon from "@jamescoyle/vue-icon";
    import {
        mdiAccountGroup,
        mdiAppleSafari,
        mdiGithub,
        mdiCow,
        mdiCreation,
        mdiCrystalBall,
        mdiRoutes,
    } from "@mdi/js";

    @Component({
        components: {
            SvgIcon,
        },
    })
    export default class ImprintView extends Vue {
        icons: Record<string, string> = {
            accountGroup: mdiAccountGroup,
            appleSafari: mdiAppleSafari,
            github: mdiGithub,
            cow: mdiCow,
            creation: mdiCreation,
            crystalBall: mdiCrystalBall,
            routes: mdiRoutes,
        };
    }
</script>

<template>

    <div id="imprint-view">
        <div class="bg-gradient-to-br from-light-blue-600 to-cyan-300 min-h-96 text-white">
            <section class="flex h-full items-end max-w-7xl mx-auto p-4 pt-64
                xl:items-center xl:px-0 xl:py-60">

                <div class="max-w-lg pr-16">
                    <div class="font-bold mb-4 text-4xl
                        xl:mb-8 xl:text-5xl">Impressum</div>
                </div>
            </section>
        </div>

        <section class="leading-relaxed max-w-7xl mx-auto p-4 space-y-8 text-blue-gray-800
            sm:space-y-16
            xl:px-0 xl:py-16">

            <div>
                <div class="font-semibold max-w-lg mb-4 pr-16 text-xl
                    xl:text-3xl">Angaben gemäß § 5 TMG</div>

                <div>
                    Yannic Bastian Rieger<br>
                    Buchenstraße 1<br>
                    85609 Aschheim
                </div>

                <div class="font-semibold my-4 pr-16 text-lg">Kontakt</div>

                <div>
                    admin@cow.network<br>
                    +49 1512 0198816
                </div>

                <div class="my-12">
                    Die Europäische Kommission stellt eine Plattform zur Online-Streitbeilegung (OS) bereit: <a class="text-rose-300" href="http://ec.europa.eu/consumers/odr">http://ec.europa.eu/consumers/odr</a>.<br>
                    Unsere E-Mail-Adresse finden Sie oben im Impressum.<br><br>
                    Wir sind nicht bereit oder verpflichtet, an Streitbeilegungsverfahren vor einer Verbraucherschlichtungsstelle teilzunehmen.
                </div>

                <div class="font-semibold my-4 pr-16 text-lg">Haftung für Inhalte</div>

                <div>
                    Als Diensteanbieter sind wir gemäß § 7 Abs.1 TMG für eigene Inhalte auf diesen Seiten nach den allgemeinen Gesetzen verantwortlich. Nach §§ 8 bis 10 TMG sind wir als Diensteanbieter jedoch nicht verpflichtet, übermittelte oder gespeicherte fremde Informationen zu überwachen oder nach Umständen zu forschen, die auf eine rechtswidrige Tätigkeit hinweisen.<br><br>
                    Verpflichtungen zur Entfernung oder Sperrung der Nutzung von Informationen nach den allgemeinen Gesetzen bleiben hiervon unberührt. Eine diesbezügliche Haftung ist jedoch erst ab dem Zeitpunkt der Kenntnis einer konkreten Rechtsverletzung möglich. Bei Bekanntwerden von entsprechenden Rechtsverletzungen werden wir diese Inhalte umgehend entfernen.
                </div>

                <div class="font-semibold my-4 pr-16 text-lg">Haftung für Links</div>

                <div>
                    Unser Angebot enthält Links zu externen Webseiten Dritter, auf deren Inhalte wir keinen Einfluss haben. Deshalb können wir für diese fremden Inhalte auch keine Gewähr übernehmen. Für die Inhalte der verlinkten Seiten ist stets der jeweilige Anbieter oder Betreiber der Seiten verantwortlich. Die verlinkten Seiten wurden zum Zeitpunkt der Verlinkung auf mögliche Rechtsverstöße überprüft. Rechtswidrige Inhalte waren zum Zeitpunkt der Verlinkung nicht erkennbar.<br><br>
                    Eine permanente inhaltliche Kontrolle der verlinkten Seiten ist jedoch ohne konkrete Anhaltspunkte einer Rechtsverletzung nicht zumutbar. Bei Bekanntwerden von Rechtsverletzungen werden wir derartige Links umgehend entfernen.
                </div>

                <div class="font-semibold my-4 pr-16 text-lg">Urheberrecht</div>

                <div>
                    Die durch die Seitenbetreiber erstellten Inhalte und Werke auf diesen Seiten unterliegen dem deutschen Urheberrecht. Die Vervielfältigung, Bearbeitung, Verbreitung und jede Art der Verwertung außerhalb der Grenzen des Urheberrechtes bedürfen der schriftlichen Zustimmung des jeweiligen Autors bzw. Erstellers. Downloads und Kopien dieser Seite sind nur für den privaten, nicht kommerziellen Gebrauch gestattet.<br><br>
                    Soweit die Inhalte auf dieser Seite nicht vom Betreiber erstellt wurden, werden die Urheberrechte Dritter beachtet. Insbesondere werden Inhalte Dritter als solche gekennzeichnet. Sollten Sie trotzdem auf eine Urheberrechtsverletzung aufmerksam werden, bitten wir um einen entsprechenden Hinweis. Bei Bekanntwerden von Rechtsverletzungen werden wir derartige Inhalte umgehend entfernen.
                </div>

                <div class="mt-12">Quelle: <a class="text-rose-300" href="https://www.e-recht24.de/">eRecht24</a></div>
            </div>

        </section>

        <footer class="bg-rose-200 text-warm-gray-800">
            <section class="max-w-7xl mx-auto px-4">
                <div class="divide-x-2 divide-rose-300 -mx-4 py-8">
                    <router-link class="px-4" :to="{ name: 'home' }">Startseite</router-link>
                    <a class="px-4" href="https://github.com/CowNetwork">Github</a>
                    <router-link class="px-4" :to="{ name: 'imprint' }">Impressum</router-link>
                </div>

                <div class="flex font-sans-alt font-medium italic items-center py-4 text-sm">
                    <img class="h-8 mr-3" src="@/assets/logo.png" />
                    <div>Made with <span class="not-italic">❤️</span> by the cows</div>
                    <div class="ml-auto">&copy; 2021 Cow Network</div>
                </div>
            </section>
        </footer>
    </div>

</template>