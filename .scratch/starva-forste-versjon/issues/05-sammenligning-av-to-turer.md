# 05: Sammenligning av to turer

**What to build:** En side som viser én tur mot en annen tur på samme strekning. For hvert punkt viser siden mellomtiden til begge turene og forskjellen. For hver etappe viser siden etappetiden til begge turene og forskjellen, og etapper der turen er tregere er røde. Besøkende kan velge en annen tur å sammenligne med, og lenken kan deles. Sammenlignings-funksjonen ligger i modulen med reglene og har tester.

Se brukerhistorie 38–50 og delene Implementation Decisions og Testing Decisions i `.scratch/starva-forste-versjon/spec.md`.

**Blocked by:** 03 (Toppliste på forsiden), fordi standardvalget bruker toppliste-funksjonen.

**Status:** ready-for-agent

- [ ] Siden viser pilotnavn, dato og antall vitner for begge turene.
- [ ] Siden viser en rad per punkt med mellomtiden til begge turene og forskjellen.
- [ ] Siden viser en rad per etappe med etappetiden til begge turene og forskjellen.
- [ ] Forskjeller vises med fortegn, for eksempel `+0:03` og `-0:01`. Forskjellen er «denne turen minus den andre turen».
- [ ] En etappe er rød bare når forskjellen er positiv.
- [ ] Uten valgt tur sammenlignes turen med rekorden. Hvis turen selv er rekorden, sammenlignes den med nummer to på topplisten.
- [ ] Hvis det ikke finnes andre turer, viser siden turen og teksten «Ingen andre turer å sammenligne med ennå».
- [ ] Listen over turer å velge har den beste turen til hver pilot og alle turene til piloten som eier turen, men ikke turen selv.
- [ ] Den valgte turen står i adressen, slik at lenken kan deles.
- [ ] Siden kan leses uten innlogging.
- [ ] Vitest-tester dekker: etappetider regnet riktig, forskjeller med riktig fortegn, rød etappe bare når turen er tregere, ingen rød etappe ved lik etappetid, og en tur sammenlignet med en identisk tur.
