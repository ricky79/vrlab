# VR Music Lab — Landing page

Quattro versioni della landing page della scuola, stessa palette nero/rosso e
stessi contenuti (titolo, descrizione, corsi, form di contatto via WhatsApp,
mappa), quattro stili diversi tra cui scegliere.

Apri `index.html` per vedere l'elenco e confrontarle, oppure apri
direttamente uno dei file:

| File | Stile |
|---|---|
| `v1-backstage.html` | Poster da concerto — font condensato, luci di scena |
| `v2-studio.html` | Editoriale, minimal — serif elegante, molto spazio |
| `v3-groove.html` | Energico e giocoso — forme rotonde, adatto anche a famiglie |
| `v4-vinyl.html` | Vintage anni '70/'80 — disco in vinile, locandina d'epoca |

Ogni file è **autonomo** (HTML/CSS/JS in un unico file, nessuna dipendenza da
installare): basta aprirlo in un browser, oppure caricarlo su un qualsiasi
hosting statico (es. GitHub Pages, Netlify, Vercel, o lo spazio web che già
usate per il sito).

## Cosa personalizzare prima di pubblicare

In **ognuno dei 4 file** ci sono 3 cose segnate con `TODO` da sostituire con i
dati reali della scuola:

1. **Numero WhatsApp** — vicino alla fine del file, nel tag `<script>`:
   ```js
   var WHATSAPP_NUMBER = "390000000000";
   ```
   Va scritto in formato internazionale, **senza** `+` e senza spazi
   (es. numero `333 123 4567` → `393331234567`).

2. **Indirizzo sulla mappa** — cercate il commento
   `<!-- TODO: sostituire "Verona" con l'indirizzo esatto della scuola -->`
   e sostituite `Verona,+VR` nell'URL della mappa con l'indirizzo reale
   (via, numero civico, città), tenendo i `+` al posto degli spazi. Es.:
   ```
   https://www.google.com/maps?q=Via+Roma+10,+Verona&output=embed
   ```
   Aggiornate anche il testo dell'indirizzo mostrato nella pagina (cercate
   "Verona, VR — indirizzo esatto in sede").

3. **Link social** — i link a Facebook e Instagram nel footer/sezione
   contatti puntano a `facebook.com/vrmusiclab` e `instagram.com/vrmusiclab`:
   verificate che siano quelli giusti.

Il form di contatto non invia dati a nessun server: al click su "Invia su
WhatsApp" apre semplicemente WhatsApp (Web o app) con un messaggio già
scritto, pronto da inviare al numero della scuola.

## Corsi inclusi

Batteria, Chitarra, Basso, Pianoforte — se cambia l'offerta corsi, cercate le
sezioni `id="corsi"` (o `#corsi` / "programma") in ciascun file.
