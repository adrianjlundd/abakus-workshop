# 01: Prosjektoppsett med strekning og eksempeldata

**What to build:** Et Next.js-prosjekt med TypeScript, Tailwind CSS, Prisma og Vitest, koblet til PostgreSQL med `DATABASE_URL` fra `.env.local`. Databasen har alle tabellene fra spesifikasjonen. Et seed-skript legger inn strekningen «Dovre på lavt nivå» og noen eksempelpiloter med turer, slik at de andre oppgavene har data å vise. Forsiden viser navnet på strekningen og punktene, hentet fra databasen.

Se `.scratch/starva-forste-versjon/spec.md`, delen Implementation Decisions, for tabellene og tidsformatet.

**Blocked by:** None (can start immediately).

**Status:** ready-for-agent

- [ ] Appen starter med én kommando, og forsiden viser «Dovre på lavt nivå» med punktene Dombås, Hjerkinn, Kongsvoll, Oppdal og Trondheim i riktig rekkefølge.
- [ ] Prisma-migreringer lager tabellene pilot, økt, strekning, punkt, tur og mellomtid.
- [ ] Punktene har en rekkefølge som er unik per strekning.
- [ ] Mellomtider lagres som hele sekunder fra start, med én rad per punkt per tur.
- [ ] Seed-skriptet legger inn strekningen og minst tre eksempelpiloter, blant dem Zorbl og Glimp, med flere turer hver. Passordene er bcrypt-hasher.
- [ ] Eksempeldataene har turer der Glimp er raskere enn Zorbl på noen etapper og tregere på andre.
- [ ] Seed-skriptet kan kjøres flere ganger uten å lage duplikater.
- [ ] Vitest er satt opp, og testkommandoen kjører.
- [ ] README eller en kommentar i prosjektet forteller hvordan man kjører migreringer, seed, appen og testene.
