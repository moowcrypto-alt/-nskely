# Ønskely.no – interaktiv designprototype

Next.js + React + TypeScript. Bygget med utgangspunkt i ønsket visuell stil.

## Kom i gang

1. Installer Node.js 20 eller nyere.
2. Kjør `npm install`.
3. Kjør `npm run dev`.
4. Åpne http://localhost:3000.

## Hva fungerer i prototypen?

Forside, mobilvennlig layout, oversikt over ønskelister, opprettelse av lister, redigering og sletting av ønsker, kategorifilter, gjestevisning, reservering, hemmelig modus og utskriftsknapp. Data lagres i `localStorage` i **samme nettleser**.

## Ikke produksjonsklar ennå

Dette er en **frontend-prototype**. Den har ikke ekte innlogging, Supabase-synkronisering, ekte deling på tvers av enheter, produktskraping, bildeopplasting, Vipps eller atomiske reservasjoner. En delingslenke i demoen viser ikke de samme dataene for andre personer. Ikke lanser dette som ferdig tjeneste.

## Videre utvikling

1. Koble Supabase Auth til konto og innlogging.
2. Lag database og Row Level Security for listeeier.
3. Implementer server-API for deling og atomisk reservasjon uten konto. Unngå å eksponere giverens navn til eieren når hemmelig modus er på.
4. Implementer sanntidsoppdatering, produktimport med manuell fallback, bilder og PDF.
5. Koble GitHub-repository til Vercel.

Miljøvariabler for Supabase kan senere settes i `.env.local`. Legg aldri service role key i klientkode.
