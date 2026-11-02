# EXILE capes

Mantelli e lista membri della fazione EXILE, letti in automatico da EXILE Client (Lunar 1.8.9 e 1.7.10 + Weave).

**Installare EXILE Client:** scarica [EXILE-Client.zip](https://github.com/esiliocloud-lang/exile-capes/releases/latest/download/EXILE-Client.zip), estrai, chiudi Lunar e fai doppio clic su `INSTALLA_EXILE.bat`. Poi si aggiorna da sola.

| Cartella / file | Contenuto |
|---|---|
| `capes/` | i mantelli. I file nella radice vanno nella cartella EXILE; ogni sottocartella è una cartella nella GUI. |
| `members.txt` | un membro per riga: `nome` oppure `nome=mantello`. |
| `manifest.json` | elenco dei file con sha1: la mod scarica solo quelli nuovi o cambiati. |
| `mod/` | l'ultima versione della mod e `latest.json`, per l'aggiornamento automatico. |

**Il modo più semplice:** la dashboard (`/admin` del servizio exile-sync), pagine *Membri* e *Mantelli*. Aggiunge e toglie membri, converte e carica i mantelli e aggiorna il manifest da sola.

**A mano:** dopo aver cambiato `capes/` o `members.txt` va rigenerato il manifest, altrimenti la mod rifiuta i file cambiati:
`py -I strumenti/mantelli/make_manifest.py <questa cartella>` (dal codice di EXILE Client), poi commit + push.

Formato dei mantelli: PNG 2:1 con larghezza multipla di 64 (64×32, 128×64 … 2048×1024).
