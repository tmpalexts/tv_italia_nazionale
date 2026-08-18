# TV italiana — Playlist M3U legale (visibile anche all'estero)

Playlist M3U con i **canali televisivi italiani in chiaro**, estratti esclusivamente
dagli **stream ufficiali** (siti web e app ufficiali dei broadcaster).

- ✅ **Legale**: nessun canale pirata, nessun canale a pagamento, nessun contenuto ridistribuito,
  nessun DRM aggirato.
- ✅ **Visibile dall'estero**: ogni link nel file principale è stato **testato da una
  connessione fuori dall'Italia** (17/08/2026) e risponde con una playlist HLS valida.
- ✅ **Funziona con VLC, Kodi, OTT Player, SSIPTV, TiviMate, IPTV Smarters** e con il
  **player web incluso** (`player.html`).

## File

| File | Contenuto |
|---|---|
| **`tv_legale`** | ✅ **Playlist principale — funziona dall'estero.** 51 canali: nazionali + feed internazionali ufficiali Rai/Mediaset + canali regionali e FAST ufficiali. |
| **`tv_italia_solo_italia.m3u8`** | 🇮🇹 Canali nazionali (Rai 1-5, Canale 5, Rete 4, Italia 1, ecc.) **geo-bloccati all'estero** — da usare solo in Italia. |
| **`player.html`** | 📱 **Web-app player** (alternativa legale a un'APK): elenco canali + riproduzione nel browser. |
| `README.md` | Questo documento. |

## Come si usa

1. **Player web (consigliato)**: apri `player.html` nel browser (oppure l'URL della live preview).
2. **VLC**: `Media → Apri file…` (o `Apri flusso di rete…` incollando il percorso) e seleziona `tv_legale`.
3. **Telefono/tablet**: apri il file con un player M3U (OTT Player, IPTV Smarters, SSIPTV, VLC).
4. **Kodi**: installa il componente IPTV Simple Client e punta al file.
5. Le righe `#EXTVLCOPT:http-user-agent=…` sono il User-Agent che il player deve inviare
   per essere accettato dal server ufficiale (VLC le applica automaticamente).

## Cosa c'è nella playlist principale (`tv_legale`) — 51 canali verificati dall'estero

### RAI — feed internazionali ufficiali (per l'estero)
| Canale | Note |
|---|---|
| Rai Italia — Europa/Africa, Nord America, Sud America, Australia | 1080p |
| Rai World Premium | 1080p |
| Rai 2 (estero) · Rai Scuola (estero) · Rai Storia (estero) | 1080p |

### Mediaset — feed internazionali ufficiali (per l'estero)
| Canale | Note |
|---|---|
| Mediaset Italia — Europa, Nord America, Australia | 1080p |

### Nazionali in chiaro
LA7 · NOVE · Real Time · DMAX · Giallo · Food Network · Super! (bambini) · Euronews Italiano ·
Cusano Italia TV · Sportitalia · Sportitalia Solocalcio · SuperTennis · TV2000 · QVC Italia ·
Padre Pio TV

### Radio TV
RTL 102.5 TV · Radio Italia TV · Deejay TV · m2o TV · Radio Capital TV · Radio Freccia ·
Radio Zeta · Radio Kiss Kiss TV · RDS Social TV · Radio Birikina TV · Radio Piter Pan TV ·
Radio Studio Delta TV

### Canali regionali e locali (stream ufficiali, non geobloccati)
Telenorba (Puglia) · TG Norba 24 (Puglia) · Antenna Sud (Puglia) · Telesveva (Puglia) ·
Radio Norba TV (Puglia) · Canale 63 Il Sole 24 Ore · Italia 53 (Lombardia) · Alma TV (Lombardia) ·
il61 (Campania) · CafèTV24 (Veneto) · MadeinBO TV (Emilia-Romagna)

### Canali FAST ufficiali
FIFA+ (calcio) · ACI Sport TV (motori)

## Perché alcuni canali "famosi" NON ci sono (nella playlist estero)

- **Canale 5, Rete 4, Italia 1, 20, Iris, La5, Cine34, Focus, Top Crime, Boing, TGCOM24,
  Italia 2, Mediaset Extra, Cartoonito, TwentySeven** → gli stream nazionali di Mediaset sono
  protetti da **DRM (Widevine)** e/o **geo-bloccati all'Italia**: non si possono guardare con
  un player normale, e **aggirare il DRM è illegale** (art. 102-quater e 171-ter L. 633/1941).
  Legalmente si vedono con l'app **Mediaset Infinity** (solo Italia). All'estero Mediaset offre
  il canale ufficiale **Mediaset Italia** (incluso).
- **Rai 1, Rai 3, Rai 4, Rai 5, Rai Movie, Rai Premium, Rai Gulp, Rai Yoyo, Rai News 24,
  Rai Sport** (versioni nazionali) → **RaiPlay è geo-bloccato all'estero** (testato: i server
  Rai rispondono con errore da fuori Italia). In Italia funzionano con
  `tv_italia_solo_italia.m3u8`. All'estero Rai mette a disposizione i feed internazionali
  inclusi (Rai Italia, Rai 2/Scuola/Storia estero).
- **TV8, Cielo, Sky TG24** → stream web Sky validi solo in Italia (file "solo Italia").
- **Radio 105 TV, R101 TV, Virgin Radio TV, Radio Montecarlo TV** → feed HbbTV Mediaset
  geo-bloccati all'Italia (file "solo Italia").

> **Perché non un APK che aggira geoblock/DRM?** Un'app che estrae o elude flussi Widevine
> sarebbe uno "strumento di elusione" di misure tecnologiche di protezione: vietato e punibile
> in Italia e nell'UE. La web-app `player.html` dà la stessa comodità (elenco + riproduzione)
> usando solo i flussi che i broadcaster mettono a disposizione legalmente.

## Verifica

- Data di verifica: **17 agosto 2026**.
- Metodo: richiesta HTTP da un indirizzo IP **fuori dall'Italia**; è considerato valido ogni
  URL che risponde con una playlist HLS valida (`#EXTM3U`/`#EXT-X-STREAM-INF`).
- Gli stream TV possono cambiare URL senza preavviso; se un canale smette di funzionare,
  controlla il sito ufficiale del broadcaster.

## EPG (guida programmi, opzionale)

- EPG iptv-org (copre la maggior parte dei tvg-id usati): <https://iptv-org.github.io/epg/>
- EPGshare IT: <https://epgshare01.online/epgshare01/epg_ripper_IT1.xml.gz>

## Nota legale

Questa raccolta **non ospita né ridistribuisce alcun contenuto**: contiene solo link pubblici
agli stream ufficiali dei rispettivi editori. La visione è consentita nei termini d'uso di
ciascun servizio (i feed internazionali Rai/Mediaset sono espressamente destinati ai telespettatori
fuori dall'Italia). Il file `tv_italia_solo_italia.m3u8` è pensato per l'uso in Italia.
