# LOTOTO — Zeker weten. Veilig werken.

Versie 4.0.0 · 4 november 2026

Nederlandstalige leeromgeving voor operators en monteurs in de procesindustrie.
De complete website staat in `dist/`. Dit is gewone HTML, CSS en JavaScript;
er is geen installatie, build, backend of database nodig.

## Publiceren via GitHub en Netlify

Koppel in het bestaande Netlify-project **lototo-industrie-website** onder
Project configuration → Build & deploy → Continuous deployment het repository
**JosvR/LOTOTO**. Selecteer:

| Instelling | Waarde |
| --- | --- |
| Production branch | `main` |
| Base directory | repository-root (`.`) |
| Package directory | leeg |
| Build command | leeg |
| Publish directory | `dist` |
| Functions directory | niet nodig |
| Environment variables | geen nodig |

`netlify.toml` legt de publicatiemap en het lege buildcommando vast.
De repositorykoppeling en productiebranch worden in Netlify ingesteld.
Na het koppelen publiceert Netlify wijzigingen op `main` automatisch.
Gebruik het bestaande project om dezelfde website-URL te behouden.
De lokale Netlify-koppeling `.netlify/` en eventuele `.env`-bestanden worden
uitgesloten van Git. Voeg geen tokens of sleutels toe aan de website.

## Gebruik en gegevens

Open `dist/index.html` of serveer de map `dist` met een lokale webserver.
De navigatie gebruikt URL-fragmenten (`#welcome`, enzovoort), dus een SPA-redirect
is niet nodig. Alle eigen bestanden hebben relatieve paden.
Lettertypen worden van Google Fonts geladen, met lokale systeemfonts als fallback.
Voortgang blijft uitsluitend in de huidige browser en op hetzelfde webadres bewaard.
Een verhuizing naar een ander domein neemt bestaande voortgang niet automatisch mee.

## Afbeelding en opleidingscontext

De landingsfoto is een AI-illustratie met een realistisch vormgegeven LOTOTO-tag.
De naam, afdeling en datum op de tag zijn fictieve voorbeeldgegevens.
Het is geen foto van een gecertificeerd product of uitvoerbaar isolatieplan.
De training ondersteunt leren; de lokale installatieprocedure en bevoegdheden
blijven bepalend voor de uitvoering op de werkplek.

De tag toont als voorbeeld J. de Vries, afdeling Technische Dienst en datum 04-11-2026. De afbeelding staat in `dist/assets/lototo-installatie-tag-v4.webp`.
