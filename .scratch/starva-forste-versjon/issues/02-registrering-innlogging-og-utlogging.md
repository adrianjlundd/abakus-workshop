# 02: Registrering, innlogging og utlogging

**What to build:** En besøkende kan registrere seg som pilot med pilotnavn og passord, og blir logget inn med en gang. En pilot kan logge inn og logge ut. Toppen av hver side viser pilotnavnet når piloten er logget inn, og ellers lenker til innlogging og registrering.

Se brukerhistorie 1–9 og 51 i `.scratch/starva-forste-versjon/spec.md`.

**Blocked by:** 01 (Prosjektoppsett med strekning og eksempeldata).

**Status:** ready-for-agent

- [ ] En besøkende kan registrere seg, blir logget inn og kommer til forsiden.
- [ ] Pilotnavnet må ha 2–30 tegn etter at mellomrom i starten og slutten er fjernet. Ellers vises en feilmelding.
- [ ] Passordet må ha minst 8 tegn. Ellers vises en feilmelding.
- [ ] Et pilotnavn som allerede finnes, uansett store eller små bokstaver, gir en feilmelding.
- [ ] Passord lagres som en bcrypt-hash, aldri i klartekst.
- [ ] Innlogging med feil pilotnavn eller feil passord gir den samme feilmeldingen.
- [ ] Innloggingen lager en økt i databasen og en cookie med `httpOnly`, `sameSite=lax` og `secure` i produksjon.
- [ ] Piloten forblir innlogget mellom sidene til økten utløper eller piloten logger ut.
- [ ] Utlogging sletter økten.
- [ ] Det finnes en funksjon på serveren som gir den innloggede piloten, eller ingen, slik at andre sider kan bruke den.
- [ ] Eksempelpilotene fra seed-skriptet kan logge inn.
