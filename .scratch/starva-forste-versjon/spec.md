# Starva: første versjon

**Status:** ready-for-agent

## Problem Statement

Zorbl er en pilot fra Kepler-22b. Zorbl har flydd strekningen «Dovre på lavt nivå» i tre hundre år, og rivalen Glimp er alltid ett sekund raskere. Zorbl vet ikke hvor på strekningen tiden går tapt: over Hjerkinn, i svingen ved Oppdal, eller et annet sted. Zorbl har heller ingen måte å vise frem turene sine på, så ingen på hjemplaneten tror på historiene. Ingen kan se hvem som er raskest, og ingen kan se om en pilot blir bedre over tid.

## Solution

Starva er en nettside der piloter registrerer seg, logger inn og legger inn turer på strekningen «Dovre på lavt nivå». En tur har en dato, en mellomtid for hvert punkt og antall vitner. Forsiden er topplisten, med den beste turen til hver pilot. Hver pilot har en offentlig pilotside med alle turene sine. For hver tur finnes en sammenligning med en annen tur, med mellomtider og etappetider side om side. Etapper der turen er tregere, er røde. Da ser Zorbl nøyaktig hvor tiden går tapt mot Glimp.

Alle kan lese topplisten, pilotsidene og sammenligningene uten å logge inn. Bare innloggede piloter kan legge inn turer.

## User Stories

1. Som besøkende vil jeg registrere meg som pilot med pilotnavn og passord, slik at jeg kan legge inn turer i mitt eget navn.
2. Som besøkende vil jeg få en feilmelding hvis pilotnavnet er tatt, slik at jeg kan velge et annet.
3. Som besøkende vil jeg få en feilmelding hvis pilotnavnet er kortere enn 2 tegn eller lengre enn 30 tegn, slik at jeg vet hva som er lov.
4. Som besøkende vil jeg få en feilmelding hvis passordet er kortere enn 8 tegn, slik at kontoen min er beskyttet.
5. Som ny pilot vil jeg bli logget inn med en gang etter registreringen og komme til forsiden, slik at jeg kan legge inn en tur uten et ekstra steg.
6. Som pilot vil jeg logge inn med pilotnavn og passord, slik at jeg kan legge inn turer.
7. Som pilot vil jeg få en feilmelding hvis pilotnavnet eller passordet er feil, uten å få vite hvilket av dem som er feil, slik at ingen kan gjette seg frem til andres pilotnavn.
8. Som pilot vil jeg logge ut, slik at ingen andre kan legge inn turer i mitt navn på maskinen min.
9. Som pilot vil jeg forbli innlogget når jeg går mellom sidene, slik at jeg ikke må logge inn hele tiden.
10. Som besøkende vil jeg se topplisten for «Dovre på lavt nivå» på forsiden, slik at jeg ser hvem som er raskest.
11. Som besøkende vil jeg at topplisten bare viser den beste turen til hver pilot, slik at én pilot ikke fyller hele listen.
12. Som besøkende vil jeg at topplisten er sortert etter totaltid, raskest først, slik at rekorden står øverst.
13. Som pilot vil jeg at den som fløy først kommer øverst ved lik totaltid, slik at den som satte tiden først får æren.
14. Som besøkende vil jeg se plassering, pilotnavn, totaltid, dato og antall vitner for hver tur på topplisten, slik at jeg får hele bildet.
15. Som besøkende vil jeg klikke på et pilotnavn på topplisten og komme til pilotsiden, slik at jeg ser alle turene til piloten.
16. Som besøkende vil jeg klikke på en tid på topplisten og komme til sammenligningen for turen, slik at jeg ser hvor turen var rask eller treg.
17. Som besøkende vil jeg se en tekst når topplisten er tom, slik at jeg forstår at ingen har lagt inn en tur ennå.
18. Som innlogget pilot vil jeg se en knapp på forsiden for å legge inn en ny tur, slik at jeg kommer raskt i gang.
19. Som besøkende vil jeg bli sendt til innloggingen hvis jeg prøver å legge inn en tur, slik at jeg forstår at jeg må logge inn først.
20. Som pilot vil jeg se punktene på strekningen i riktig rekkefølge når jeg legger inn en tur, slik at jeg vet hvilken mellomtid som hører til hvilket punkt.
21. Som pilot vil jeg skrive inn hver mellomtid som minutter og sekunder, for eksempel `4:12`, slik at det går raskt.
22. Som pilot vil jeg få en feilmelding hvis en mellomtid mangler, slik at turen blir komplett.
23. Som pilot vil jeg få en feilmelding hvis en mellomtid ikke er større enn den forrige, slik at jeg ser at jeg har skrevet feil.
24. Som pilot vil jeg få en feilmelding hvis en mellomtid har feil format, for eksempel `4:75` eller `abc`, slik at jeg kan rette den.
25. Som pilot vil jeg velge datoen for turen, med dagens dato valgt fra start, slik at jeg også kan legge inn gamle turer.
26. Som pilot vil jeg få en feilmelding hvis datoen er i fremtiden, slik at ingen jukser med datoer.
27. Som pilot vil jeg skrive inn antall vitner, 0 eller mer, slik at alle ser at turen er ekte.
28. Som pilot vil jeg få en feilmelding hvis antall vitner er negativt eller ikke et helt tall, slik at tallet gir mening.
29. Som pilot vil jeg at alle feilene i skjemaet vises samtidig, og at det jeg skrev blir stående, slik at jeg kan rette alt på en gang.
30. Som pilot vil jeg komme til sammenligningen for den nye turen når jeg har lagret den, slik at jeg ser med en gang hvordan den gikk mot rekorden.
31. Som pilot vil jeg at en lagret tur ikke kan endres eller slettes, slik at ingen kan jukse ved å endre tider etterpå.
32. Som besøkende vil jeg se en pilotside for hver pilot, med alle turene til piloten, slik at jeg ser hvordan piloten har utviklet seg.
33. Som besøkende vil jeg at turene på pilotsiden er sortert med nyeste dato først, slik at jeg ser de siste turene øverst.
34. Som besøkende vil jeg se dato, totaltid og antall vitner for hver tur på pilotsiden, slik at jeg kan sammenligne turene.
35. Som pilot vil jeg se også mine dårlige turer på pilotsiden, slik at jeg ser om jeg blir bedre.
36. Som besøkende vil jeg klikke på en tur på pilotsiden og komme til sammenligningen for turen, slik at jeg ser detaljene.
37. Som besøkende vil jeg se en tekst når en pilot ikke har noen turer, slik at siden ikke ser tom og ødelagt ut.
38. Som besøkende vil jeg se en tur sammenlignet med en annen tur på samme strekning, slik at jeg ser forskjellen.
39. Som besøkende vil jeg se mellomtiden til begge turene ved hvert punkt, og forskjellen, slik at jeg ser hvor langt bak eller foran turen ligger.
40. Som besøkende vil jeg se etappetiden til begge turene for hver etappe, og forskjellen, slik at jeg ser hvor tiden går tapt.
41. Som pilot vil jeg at etapper der turen min er tregere er røde, slik at jeg ser det med en gang.
42. Som besøkende vil jeg at forskjellene vises med fortegn, for eksempel `+0:03` og `-0:01`, slik at jeg ser hvem som var raskest.
43. Som besøkende vil jeg at rekorden er valgt fra start i sammenligningen, slik at jeg ser turen mot den beste med en gang.
44. Som rekordholder vil jeg at turen nummer to på topplisten er valgt fra start når jeg åpner rekordturen min, slik at turen ikke blir sammenlignet med seg selv.
45. Som besøkende vil jeg se en tekst når det ikke finnes andre turer å sammenligne med, slik at jeg forstår hvorfor tabellen mangler.
46. Som besøkende vil jeg velge en annen tur å sammenligne med, fra en liste med den beste turen til hver pilot og alle turene til piloten som eier turen, slik at jeg kan sammenligne med hvem jeg vil.
47. Som pilot vil jeg sammenligne en tur med en av mine egne tidligere turer, slik at jeg ser om jeg er raskere enn før.
48. Som pilot vil jeg sammenligne turen min med turen til en bestemt rival, slik at jeg ser hvor Glimp er raskere enn meg.
49. Som besøkende vil jeg se pilotnavn, dato og antall vitner for begge turene i sammenligningen, slik at jeg vet hvilke turer jeg ser på.
50. Som besøkende vil jeg kunne dele lenken til en sammenligning, slik at jeg kan vise den til hele hjemplaneten.
51. Som besøkende vil jeg se pilotnavnet mitt i toppen av siden når jeg er logget inn, og ellers lenker til innlogging og registrering, slik at jeg vet om jeg er logget inn.

## Implementation Decisions

- Stakken er Next.js med TypeScript og App Router, Tailwind CSS for utseende, og PostgreSQL med Prisma. Tilkoblingen bruker `DATABASE_URL` fra `.env.local`.
- Databasen har disse tabellene:
  - Pilot: id, pilotnavn (unikt), passordhash, opprettet.
  - Økt: id (en tilfeldig, lang nøkkel), pilot, utløper.
  - Strekning: id, navn.
  - Punkt: id, strekning, navn, rekkefølge (unik per strekning).
  - Tur: id, pilot, strekning, dato, antall vitner, opprettet.
  - Mellomtid: tur, punkt, sekunder (heltall). Én rad per punkt per tur.
- Tider lagres som hele sekunder fra start. Visningen og skjemaet bruker formatet `m:ss`, for eksempel `4:12`. Minuttene kan være flere enn 59.
- Startpunktet har mellomtid 0, og piloten fyller den ikke inn. Piloten fyller inn mellomtid for Hjerkinn, Kongsvoll, Oppdal og Trondheim. Mellomtiden ved Trondheim er totaltiden.
- Prisma-migreringer lager tabellene. Et seed-skript legger inn strekningen «Dovre på lavt nivå» med punktene Dombås, Hjerkinn, Kongsvoll, Oppdal og Trondheim, i den rekkefølgen. Seed-skriptet kan kjøres flere ganger uten å lage duplikater.
- Første versjon har bare én strekning. Koden henter likevel strekningen fra databasen og antar ikke punktene, slik at flere strekninger senere ikke krever ny modell.
- Reglene i Starva ligger i én egen modul uten avhengighet til databasen, Next.js eller nettleseren. Modulen har tre funksjoner:
  - Sjekk av en ny tur: tar inn punktene på strekningen, mellomtidene som tekst, datoen, antall vitner og dagens dato. Den svarer enten med en gyldig tur (mellomtider i sekunder) eller med en liste over feil, knyttet til hvert felt.
  - Sammenligning av to turer: tar inn punktene på strekningen og to turer. Den gir en rad per punkt med mellomtiden til begge og forskjellen, og en rad per etappe med etappetiden til begge, forskjellen og om turen er tregere.
  - Toppliste: tar inn alle turene på en strekning. Den gir den beste turen til hver pilot, sortert etter totaltid. Ved lik totaltid kommer turen med tidligst dato først. Ved lik dato kommer turen som ble lagret først.
- Forskjeller regnes som «denne turen minus den andre turen». En positiv forskjell betyr at denne turen er tregere. En etappe er rød når forskjellen er positiv.
- Datoen er en kalenderdato uten klokkeslett. Dagens dato sendes inn til sjekken, slik at sjekken ikke leser klokken selv.
- Passord lagres som en bcrypt-hash. Innloggingen lager en økt i databasen og legger nøkkelen i en cookie med `httpOnly`, `sameSite=lax` og `secure` i produksjon. Utlogging sletter økten. Ingen bibliotek for innlogging.
- Pilotnavnet må ha mellom 2 og 30 tegn etter at mellomrom i starten og slutten er fjernet. Sjekken for unike pilotnavn skiller ikke mellom store og små bokstaver.
- Registrering, innlogging, utlogging og lagring av en tur bruker server actions eller route handlers. Lagring av en tur sjekker innloggingen på serveren, ikke bare i nettleseren.
- En tur og mellomtidene lagres i én transaksjon.
- Det finnes ingen måte å endre eller slette en tur på.
- Sidene er:
  - Forsiden: topplisten for strekningen, og en knapp for å legge inn en ny tur.
  - Registrering og innlogging.
  - Ny tur: skjemaet, bare for innloggede piloter.
  - Pilotside: alle turene til én pilot, nyeste dato først.
  - Sammenligning: én tur mot en annen tur. Den andre turen står i adressen (for eksempel som en parameter), slik at lenken kan deles. Uten parameter gjelder standardvalget: rekorden, eller nummer to på topplisten hvis turen selv er rekorden.
- Listen over turer å sammenligne med har den beste turen til hver pilot og alle turene til piloten som eier turen. Turen selv er ikke med.

## Testing Decisions

- En god test sjekker det modulen gir ut for et gitt inndata, ikke hvordan modulen regner det ut. Testene kaller bare de tre funksjonene i modulen med reglene.
- Testene bruker Vitest og trenger ingen database og ingen nettleser.
- Sjekken av en ny tur testes for: gyldig tur, mellomtid som mangler, mellomtid med feil format (`4:75`, `abc`, tom tekst), mellomtider som ikke øker (også like mellomtider), dato i fremtiden, dagens dato (gyldig), negativt antall vitner, antall vitner som ikke er et helt tall, og flere feil samtidig.
- Sammenligningen testes for: etappetider regnet riktig, forskjeller med riktig fortegn, rød etappe bare når turen er tregere, ingen rød etappe ved lik etappetid, og en tur sammenlignet med en identisk tur.
- Topplisten testes for: bare den beste turen per pilot, sortering etter totaltid, lik totaltid avgjort av dato, lik dato avgjort av når turen ble lagret, og en tom liste.
- Repoet har ingen tester fra før. Disse testene er de første.
- Innlogging, skjemaer, databasen og sidene testes ved å bruke appen.

## Out of Scope

- Kart og ruten som en strek på et kart.
- Feed med turer fra venner, og varsel om ny rekord.
- Melding om juks, merke på meldte turer og oppsynspilot.
- Nye strekninger, og godkjenning av dem.
- Vitner fordelt på typer, som turister, bønder, elger og politifolk.
- Stråler, kommentarer og bilder av kornsirkler.
- Endring og sletting av turer.
- Glemt passord, e-post og innlogging med stemmeavtrykk.
- Romtemaet, hvis tiden ikke strekker til.

## Further Notes

- Ordene i spesifikasjonen følger `GLOSSARY.md`: pilot, strekning, punkt, etappe, tur, mellomtid, etappetid, totaltid, toppliste, rekord og antall vitner.
- Kundesamtalen med Zorbl prioriterte å se hvor tiden går tapt. Hvis tiden blir knapp, er sammenligningen viktigere enn pilotsiden.
- Starva har et tema med romvesener og flygende tallerkener. Hold designet enkelt først, og legg til romtemaet til slutt.
