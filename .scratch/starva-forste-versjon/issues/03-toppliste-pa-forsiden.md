# 03: Toppliste på forsiden

**What to build:** Forsiden viser topplisten for «Dovre på lavt nivå»: den beste turen til hver pilot, sortert etter totaltid. Hver rad viser plassering, pilotnavn, totaltid, dato og antall vitner. Toppliste-funksjonen ligger i modulen med reglene, uten avhengighet til databasen eller Next.js, og har tester.

Se brukerhistorie 10–18 og delene Implementation Decisions og Testing Decisions i `.scratch/starva-forste-versjon/spec.md`.

**Blocked by:** 01 (Prosjektoppsett med strekning og eksempeldata).

**Status:** ready-for-agent

- [ ] Topplisten viser bare den beste turen til hver pilot.
- [ ] Topplisten er sortert etter totaltid, raskest først.
- [ ] Ved lik totaltid kommer turen med tidligst dato først, og ved lik dato turen som ble lagret først.
- [ ] Tider vises som `m:ss`, for eksempel `4:12`.
- [ ] Pilotnavnet lenker til pilotsiden, og tiden lenker til sammenligningen for turen.
- [ ] En tom toppliste viser en tekst om at ingen har lagt inn en tur ennå.
- [ ] Forsiden har en knapp for å legge inn en ny tur.
- [ ] Vitest-tester dekker: bare den beste turen per pilot, sortering etter totaltid, lik totaltid avgjort av dato, lik dato avgjort av når turen ble lagret, og en tom liste.
