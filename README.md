# EXILE capes

Mantelli e lista membri della fazione EXILE, letti in automatico da EXILE Client (Lunar 1.8.9 + Weave).

- `capes/` — i mantelli. Ogni sottocartella è una categoria nella GUI.
- `members.txt` — un membro per riga, `nome` oppure `nome=mantello`.
- `manifest.json` — elenco dei file con sha1: la mod scarica solo quelli nuovi o cambiati.

Per aggiungere o cambiare un mantello: metti il file in `capes/`, rigenera il manifest
(`py -I tools/make_manifest.py <questa cartella>` dal progetto ExileCapes) e fai commit + push.
