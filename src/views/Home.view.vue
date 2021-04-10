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
    export default class HomeView extends Vue {
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

    <div id="home-view">
        <div class="bg-gradient-to-br from-light-blue-600 to-cyan-300 min-h-96 text-white">
            <section class="flex h-full items-end max-w-7xl mx-auto p-4 pt-64
                xl:items-center xl:px-0 xl:py-60">

                <div class="max-w-lg pr-16">
                    <div class="font-bold mb-4 text-4xl
                        xl:mb-8 xl:text-5xl">Muhhhhh, wir sind das Cow Network</div> <!-- Maybe skew + rotate? -->

                    <div class="font-handwriting text-2xl
                        xl:text-3xl">Bei uns sind die Visionen klein,<br>dafür die Euter umso größer.</div> <!-- Maybe rotate as well? -->
                </div>
            </section>
        </div>

        <section class="leading-relaxed max-w-7xl mx-auto p-4 space-y-16 text-blue-gray-800
            xl:px-0 xl:py-16">

            <div class="gap-16 grid grid-cols-2">
                <div class="py-8 self-center">
                    <div class="bg-yellow-400 inline-block p-2 rounded">
                        <svg-icon :path="icons.cow" :size="32" type="mdi" />
                    </div>

                    <div class="font-sans-alt font-semibold italic mb-4 mt-4 text-3xl">Was ist das Cow Network?</div>
                    <div class="font-light text-lg">Wir sind ein professioneller Trashserver&trade;, der es sich zur Aufgabe gemacht hat, die üblichen Erwartungen an einen Minecraft-Server einfach komplett zu ignorieren.</div>
                </div>
                <div class="bg-gradient-to-br from-yellow-400 to-amber-500 h-80 rounded-lg shadow-lg"></div>
            </div>

            <div class="gap-16 grid grid-cols-2">
                <div class="bg-gradient-to-br from-lime-400 to-emerald-500 h-80 rounded-lg shadow-lg"></div>
                <div class="py-8 self-center">
                    <div class="bg-green-400 inline-block p-2 rounded">
                        <svg-icon :path="icons.crystalBall" :size="32" type="mdi" />
                    </div>

                    <div class="font-sans-alt font-semibold italic mb-4 mt-4 text-3xl">Wie funktioniert das ohne Visionen?</div>
                    <div class="font-light text-lg">Unser einziges Ziel ist es eine Umgebung zu erschaffen, in der unserer Kreativität keine Grenzen gesetzt sind. Das Cow Network ist eine Spielwiese auf der wir uns ohne Verpflichtungen austoben können.</div>
                </div>
            </div>

            <div class="gap-16 grid grid-cols-2">
                <div class="py-8 self-center">
                    <div class="bg-rose-400 inline-block p-2 rounded">
                        <svg-icon :path="icons.appleSafari" :size="32" type="mdi" />
                    </div>

                    <div class="font-sans-alt font-semibold italic mb-4 mt-4 text-3xl">Welche Features kann ich erwaten?</div>
                    <div class="font-light text-lg">Erwarte am besten gar nichts. Jeder hat seine eigenen Ideen und es wird definitiv einigen geilen Scheiß geben, aber wir machen nur das, wozu wir Lust haben.</div>
                </div>
                <div class="bg-gradient-to-br from-red-400 to-rose-500 h-80 rounded-lg shadow-lg"></div>
            </div>

            <div class="gap-16 grid grid-cols-4">
                <div>
                    <div class="bg-cyan-400 inline-block p-2 rounded">
                        <svg-icon :path="icons.github" :size="32" type="mdi" />
                    </div>

                    <div class="font-sans-alt font-semibold italic mb-8 mt-4 text-2xl">100% Transparenz und Open-Source</div>
                    <div class="font-light text-lg">Unsere gesamte Software ist für die Open-Source-Community unter der GPL Lizenz (oder eines ihrer Derivate) auf GitHub verfügbar.</div>
                </div>

                <div>
                    <div class="bg-cyan-400 inline-block p-2 rounded">
                        <svg-icon :path="icons.creation" :size="32" type="mdi" />
                    </div>

                    <div class="font-sans-alt font-semibold italic mb-8 mt-4 text-2xl">Cutting Edge Technology&trade;</div>
                    <div class="font-light text-lg">Wir wollen den Fortschritt nicht aufhalten. Das Cow Network läuft wenn möglich immer auf der neuesten Minecraft Version.</div>
                </div>

                <div>
                    <div class="bg-cyan-400 inline-block p-2 rounded">
                        <svg-icon :path="icons.accountGroup" :size="32" type="mdi" />
                    </div>

                    <div class="font-sans-alt font-semibold italic mb-8 mt-4 text-2xl">Ein Platz zum Wohlfühlen und Spaß haben</div>
                    <div class="font-light text-lg">Wir machen das Cow Network prinzipiell für uns selbst, aber jeder ist willkommen, um mit Freunden hier eine tolle Zeit zu verbringen.</div>
                </div>

                <div>
                    <div class="bg-cyan-400 inline-block p-2 rounded">
                        <svg-icon :path="icons.routes" :size="32" type="mdi" />
                    </div>

                    <div class="font-sans-alt font-semibold italic mb-8 mt-4 text-2xl">Anders aus Überzeugung, Einzigartig by Design</div>
                    <div class="font-light text-lg">Minecraft Server unterscheiden sich heute kaum noch voneinander. Wir wollen nicht das nächste Copy-Paste-PvP-Netzwerk werden.</div>
                </div>
            </div>
        </section>

        <div class="bg-gradient-to-br from-light-blue-900 to-teal-900 shadow-inner text-white">
            <section class="max-w-7xl mx-auto py-16">
                <div class="font-bold max-w-lg pr-16 text-3xl
                    xl:text-4xl" style="transform: skew(-10deg) rotate(-4deg)">Diese geilen Kühe<br>machen sich die Mühe...</div>

                <div class="grid grid-cols-7 py-16">
                    <div class="relative mt-12">
                        <img src="https://visage.surgeplay.com/full/256/99f5efbb-046f-4086-9a57-647959953d1f" />
                        <div class="absolute font-handwriting text-3xl" style="bottom: -48px; left: -20px">Benedikt</div>
                        <div class="absolute font-handwriting text-4xl" style="bottom: -36px; left: 80px">)</div>
                        <div class="absolute font-handwriting text-4xl" style="bottom: -28px; left: 82px; transform: rotate(-20deg)">^</div>
                    </div>
                    <div class="relative mt-8">
                        <img src="https://visage.surgeplay.com/full/256/42fa7a75-7afa-4a19-932a-1c385c07048a" />
                        <div class="absolute font-handwriting text-3xl" style="top: -48px">Daniel</div>
                        <div class="absolute font-handwriting text-4xl" style="left: 80px; top: -40px; transform: rotate(-48deg)">)</div>
                        <div class="absolute font-handwriting text-4xl" style="left: 90px; top: -32px; transform: rotate(180deg)">^</div>
                    </div>
                    <div class="relative mt-4">
                        <img src="https://visage.surgeplay.com/full/256/cfe6cfe7-640b-4412-a1e6-107ac18be0aa" />
                        <div class="absolute font-handwriting text-3xl" style="bottom: -24px; left: 20px">Fabian</div>
                        <div class="absolute font-handwriting text-4xl" style="bottom: 0px; left: 80px">)</div>
                        <div class="absolute font-handwriting text-4xl" style="bottom: 14px; left: 87px; transform: rotate(76deg)">&lt;</div>
                    </div>
                    <div class="relative">
                        <img src="https://visage.surgeplay.com/full/256/4bb8bd7c-c55d-4232-9529-d4d392de0361" />
                        <div class="absolute font-handwriting text-3xl" style="left: 64px; top: -72px">Lukas</div>
                        <div class="absolute font-handwriting text-4xl" style="left: 80px; top: -40px">/</div>
                        <div class="absolute font-handwriting text-4xl" style="left: 82px; top: -32px; transform: scaleX(-1) rotate(-32deg)">v</div>
                    </div>
                    <div class="relative -mt-4">
                        <img src="https://visage.surgeplay.com/full/256/afbae935-a146-41df-b969-b431f12cdbbe" />
                        <div class="absolute font-handwriting text-3xl" style="bottom: 10px; right: 48px">Pia</div>
                        <div class="absolute font-handwriting text-4xl" style="bottom: 24px; right: 90px">\</div>
                        <div class="absolute font-handwriting text-4xl" style="bottom: 30px; left: 77px; transform: rotate(-100deg)">&gt;</div>
                    </div>
                    <div class="relative -mt-8">
                        <img src="https://visage.surgeplay.com/full/256/2d30be41-1c6f-4758-911e-c60912cd16ca" />
                        <div class="absolute font-handwriting text-3xl" style="right: 32px; top: -64px">Tobi</div>
                        <div class="absolute font-handwriting text-4xl" style="left: 80px; top: -48px; transform: rotate(4deg)">(</div>
                        <div class="absolute font-handwriting text-4xl" style="left: 76px; top: -34px; transform: rotate(267deg)">&lt;</div>
                    </div>
                    <div class="relative -mt-12">
                        <img src="https://visage.surgeplay.com/full/256/92de217b-8b2b-403b-86a5-fe26fa3a9b5f" />
                        <div class="absolute font-handwriting text-3xl" style="bottom: 52px; right: 0px">Yannic</div>
                        <div class="absolute font-handwriting text-4xl" style="bottom: 44px; left: 80px; transform: rotate(-48deg)">(</div>
                        <div class="absolute font-handwriting text-4xl" style="bottom: 56px; left: 74px; transform: rotate(-16deg)">^</div>
                    </div>
                </div>
            </section>
        </div>

        <section class="leading-relaxed max-w-7xl mx-auto p-4 space-y-16 text-blue-gray-800
            xl:px-0 xl:py-16">

            <div>
                <div class="font-handwriting mb-2 text-xl">FA-KUH, hihi</div>
                <div class="font-semibold max-w-lg pr-16 text-3xl">Antworten auf Fragen, von denen wir glauben, dass sie häufig gestellt werden könnten</div>
            </div>

            <div class="gap-16 grid grid-cols-3">
                <div>
                    <div class="font-sans-alt font-semibold italic mb-4 text-xl">Seid ihr der Nachfolger von RewisServer?</div>
                    <div class="font-light text-lg">&mdash; Zum Glück nicht.</div>
                </div>

                <div>
                    <div class="font-sans-alt font-semibold italic mb-4 text-xl">Wann gehts los?</div>
                    <div class="font-light text-lg">&mdash; Hoffentlich bald schon!</div>
                </div>

                <div>
                    <div class="font-sans-alt font-semibold italic mb-4 text-xl">Macht ihr auch...?</div>
                    <div class="font-light text-lg">&mdash; Vermutlich nein.</div>
                </div>

                <div>
                    <div class="font-sans-alt font-semibold italic mb-4 text-xl">Aber ihr könntet doch...!</div>
                    <div class="font-light text-lg">&mdash; Nö.</div>
                </div>

                <div>
                    <div class="font-sans-alt font-semibold italic mb-4 text-xl">Kann ich mich als Supporter/Moderator bewerben?</div>
                    <div class="font-light text-lg">&mdash; Wir versuchen kein riesiges Team aufzubauen. Für Supporter/Moderatoren haben wir kein Bedarf.</div>
                </div>

                <div>
                    <div class="font-sans-alt font-semibold italic mb-4 text-xl">Was ist wenn jemand cheatet oder beleidigt?</div>
                    <div class="font-light text-lg">&mdash; Da kennen wir keine Toleranz. Wer sich falsch verhält wird permanent gebannt.</div>
                </div>

                <div>
                    <div class="font-sans-alt font-semibold italic mb-4 text-xl">Ich spiele eure Modi nicht gerne!!1!1</div>
                    <div class="font-light text-lg">&mdash; Dann lass es.</div>
                </div>

                <div>
                    <div class="font-sans-alt font-semibold italic mb-4 text-xl">Ich will aber lieber PvP spielen!!1!1</div>
                    <div class="font-light text-lg">&mdash; PvP können andere Netzwerke besser, keiner zwingt dich hier zu bleiben.</div>
                </div>

                <div>
                    <div class="font-sans-alt font-semibold italic mb-4 text-xl">Warum liegt hier Stroh?</div>
                    <div class="font-light text-lg">&mdash; Hoffentlich hast du ne Maske auf!</div>
                </div>
            </div>
        </section>

        <footer class="bg-rose-200 text-rose-500">
            <section class="max-w-7xl mx-auto">
                <!-- <div class="divide-x-2 divide-rose-300 -mx-4 py-8">
                    <a class="px-4">Website</a>
                    <a class="px-4">Github</a>
                </div> -->

                <div class="flex font-sans-alt font-medium italic items-center py-4 text-rose-500 text-sm">
                    <img class="h-8 mr-3" src="https://cow.network/CowDab-250.png" />
                    <div>Made with <span class="not-italic">❤️</span> by the cows</div>
                    <div class="ml-auto">&copy; 2021 Cow Network</div>
                </div>
            </section>
        </footer>
    </div>

</template>