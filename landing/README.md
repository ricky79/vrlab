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

## Dati già inseriti

- **WhatsApp:** +39 340 267 8814
- **Sede:** Via Beniamino Romagnoli 13, Verona (VR) — se la città non è
  Verona, cercate `Via+Beniamino+Romagnoli+13,+Verona,+VR` in ciascun file
  (URL della mappa) e il testo "Via Beniamino Romagnoli 13, Verona (VR)" e
  correggete la città.
- **Logo:** `vrlab.png`, nella root del progetto (un livello sopra questa
  cartella `landing/`). Ogni pagina lo richiama con il percorso relativo
  `../vrlab.png`, sia nel logo in alto sia come favicon. Se spostate il file
  immagine, aggiornate quel percorso in tutte le pagine.
- **Social:** i link a Facebook e Instagram nel footer/sezione contatti
  puntano a `facebook.com/vrmusiclab` e `instagram.com/vrmusiclab`:
  verificate che siano quelli giusti.

Il numero WhatsApp è impostato vicino alla fine di ogni file, nel tag
`<script>`:
```js
var WHATSAPP_NUMBER = "393402678814";
```
(formato internazionale, senza `+` e senza spazi — utile saperlo se in
futuro il numero cambia).

Il form di contatto non invia dati a nessun server: al click su "Invia su
WhatsApp" apre semplicemente WhatsApp (Web o app) con un messaggio già
scritto, pronto da inviare al numero della scuola.

## Corsi inclusi

Batteria, Chitarra, Basso, Pianoforte — se cambia l'offerta corsi, cercate le
sezioni `id="corsi"` (o `#corsi` / "programma") in ciascun file.
