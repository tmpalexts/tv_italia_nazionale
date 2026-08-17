# TV italiana — Playlist M3U legale (visibile anche all'estero)

Playlist M3U con i **principali canali televisivi italiani in chiaro**, estratti
esclusivamente dagli **stream ufficiali** (siti web e app ufficiali dei broadcaster).

- ✅ **Legale**: nessun canale pirata, nessun canale a pagamento, nessun contenuto ridistribuito.
- ✅ **Visibile dall'estero**: ogni link nel file principale è stato **testato da una
  connessione fuori dall'Italia** (17/08/2026) e risponde con una playlist HLS valida.
- ✅ **Funziona con VLC, Kodi, OTT Player, SSIPTV, TiviMate, IPTV Smarters**, ecc.

## File

| File | Contenuto |
|---|---|
| **`tv_legale`** | ✅ **Playlist principale — funziona dall'estero.** Canali nazionali + feed internazionali ufficiali di Rai e Mediaset per gli italiani all'estero. |
| **`tv_italia_solo_italia.m3u8`** | 🇮🇹 Canali nazionali (Rai 1-5, Canale 5, Rete 4, Italia 1, ecc.) **geo-bloccati all'estero** — da usare solo in Italia. |
| `README.md` | Questo documento. |

## Come si usa

1. **VLC**: `Media → Apri file…` (o `Apri flusso di rete…` incollando il percorso) e seleziona `tv_legale`.
2. **Telefono/tablet**: apri il file con un player M3U (OTT Player, IPTV Smarters, SSIPTV, VLC).
3. **Kodi**: installa il componente IPTV Simple Client e punta al file.
4. Alcuni canali hanno una riga `#EXTVLCOPT:http-user-agent=…`: è il User-Agent che il player
   deve inviare per essere accettato dal server ufficiale (VLC la legge automaticamente).

## Cosa c'è nella playlist principale (`tv_legale`) e da dove viene

| Canale | Fonte ufficiale | Note |
|---|---|---|
| Rai Italia (EU / Nord America / Sud America / Australia) | Distribuzione internazionale Rai per l'estero | 1080p, programma Rai dedicato agli italiani all'estero |
| Rai World Premium | Distribuzione internazionale Rai | Serie/eventi Rai |
| Rai 2 · Rai Scuola · Rai Storia (feed estero) | Distribuzione internazionale Rai | Versioni per l'estero, visibili fuori dall'Italia |
| Mediaset Italia (EU / Nord America / Australia) | Distribuzione internazionale Mediaset | Feed ufficiale Mediaset per l'estero |
| LA7 | la7.it — diretta | 720p |
| NOVE · Real Time · DMAX · Giallo · Food Network | discovery+ / siti ufficiali Warner Bros. Discovery | Canali in chiaro, 1080p |
| Super! | Sky (canale gratuito) | Bambini |
| Euronews Italiano | euronews.com — diretta | 720p |
| Sportitalia | sportitalia.com | 1080p |
| SuperTennis | supertennis.tv | 1080p |
| RTL 102.5 TV · Radio Freccia · Radio Zeta | App/sito RTL 102.5 | 1080p |
| Radio Italia TV | radioitalia.it | |
| Deejay TV · m2o TV · Radio Capital TV | App Radio Deejay / Radio Capital / m2o | 1080p |
| Radio Kiss Kiss TV | kisskiss.it | |
| RDS Social TV | rds.it | 1080p |
| TV2000 | tv2000.it | 1080p |
| QVC Italia | qvc.it | |
| Padre Pio TV | padrepiotv.it | 1080p |

## Perché alcuni canali "famosi" NON ci sono (nella playlist estero)

- **Canale 5, Rete 4, Italia 1, 20, Iris, La5, Cine34, Focus, Top Crime, Boing, TGCOM24,
  Italia 2, Mediaset Extra, Cartoonito, TwentySeven** → gli stream nazionali di Mediaset sono
  protetti da **DRM (Widevine)** e/o **geo-bloccati all'Italia**: non si possono guardare con
  un player normale. Legalmente si vedono solo con l'app **Mediaset Infinity** (solo Italia).
  All'estero Mediaset offre il canale ufficiale **Mediaset Italia** (incluso) e i programmi su
  Mediaset Infinity/piattaforme internazionali.
- **Rai 1, Rai 3, Rai 4, Rai 5, Rai Movie, Rai Premium, Rai Gulp, Rai Yoyo, Rai News 24,
  Rai Sport** (versioni nazionali) → il servizio **RaiPlay è geo-bloccato all'estero**
  (testato: i server Rai rispondono con errore da fuori Italia). In Italia funzionano con il
  file `tv_italia_solo_italia.m3u8`. All'estero Rai mette a disposizione i feed internazionali
  inclusi nella playlist principale (Rai Italia, Rai 2/Scuola/Storia estero).
- **TV8, Cielo, Sky TG24** → stream web Sky validi solo in Italia (inclusi nel file
  "solo Italia"; il token di accesso scade il 19/12/2027).
- **Radio 105 TV, R101 TV, Virgin Radio TV, Radio Montecarlo TV** → feed HbbTV Mediaset
  geo-bloccati all'Italia (nel file "solo Italia").
- **DMAX, Real Time, Giallo, K2, Frisbee, Boing** sui vecchi elenchi → i vecchi link Akamai
  sono morti; oggi i canali WBD in chiaro si vedono con gli stream ufficiali inclusi (NOVE,
  Real Time, DMAX, Giallo, Food Network) o con l'app **Discovery+/Dplay**.

In sintesi: se un broadcaster distribuisce legalmente all'estero, il link è nella playlist
principale; se è riservato all'Italia, sta nel file "solo Italia".

## Verifica

- Data di verifica: **17 agosto 2026**.
- Metodo: richiesta HTTP da un indirizzo IP **fuori dall'Italia**; è considerato valido ogni
  URL che risponde con una playlist HLS (`#EXTM3U`/`#EXT-X-STREAM-INF`) anche con più qualità.
- Gli stream TV possono cambiare URL senza preavviso; se un canale smette di funzionare,
  controlla il sito ufficiale del broadcaster (tabella sopra).

## EPG (guida programmi, opzionale)

Puoi agganciare una guida TV gratuita ai player che la supportano, per esempio:
- EPG iptv-org (copre la maggior parte dei tvg-id usati): <https://iptv-org.github.io/epg/>
- EPGshare IT: <https://epgshare01.online/epgshare01/epg_ripper_IT1.xml.gz>

## Nota legale

Questa raccolta **non ospita né ridistribuisce alcun contenuto**: contiene solo link pubblici
agli stream ufficiali dei rispettivi editori. La visione è consentita nei termini d'uso di
ciascun servizio (i feed internazionali Rai/Mediaset sono espressamente destinati ai telespettatori
fuori dall'Italia). Il file `tv_italia_solo_italia.m3u8` è pensato per l'uso in Italia.
