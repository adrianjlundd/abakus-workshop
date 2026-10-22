# 06: Legg inn en tur

**What to build:** En innlogget pilot fyller ut et skjema med dato, en mellomtid for hvert punkt etter start og antall vitner, og lagrer turen. Etter lagring kommer piloten til sammenligningen for den nye turen. Sjekken av en ny tur ligger i modulen med reglene og har tester.

Se brukerhistorie 18–31 og delene Implementation Decisions og Testing Decisions i `.scratch/starva-forste-versjon/spec.md`.

**Blocked by:** 02 (Registrering, innlogging og utlogging) og 05 (Sammenligning av to turer).

**Status:** ready-for-agent

- [ ] En besøkende som ikke er logget inn, blir sendt til innloggingen.
- [ ] Skjemaet viser punktene på strekningen i riktig rekkefølge. Startpunktet har mellomtid 0 og fylles ikke inn.
- [ ] Mellomtider skrives som `m:ss`. Minuttene kan være flere enn 59.
- [ ] Datoen er dagens dato fra start. En dato i fremtiden gir en feilmelding.
- [ ] Antall vitner må være et helt tall, 0 eller mer.
- [ ] En mellomtid som mangler, har feil format, eller ikke er større enn den forrige, gir en feilmelding ved feltet.
- [ ] Alle feilene vises samtidig, og det piloten skrev blir stående.
- [ ] Serveren sjekker innloggingen og turen på nytt før lagring.
- [ ] Turen og mellomtidene lagres i én transaksjon.
- [ ] Etter lagring kommer piloten til sammenligningen for den nye turen. Turen vises på pilotsiden, og på topplisten hvis den er pilotens beste.
- [ ] Det finnes ingen måte å endre eller slette en lagret tur på.
- [ ] Vitest-tester dekker: gyldig tur, mellomtid som mangler, feil format (`4:75`, `abc`, tom tekst), mellomtider som ikke øker (også like), dato i fremtiden, dagens dato, negativt antall vitner, antall vitner som ikke er et helt tall, og flere feil samtidig.
