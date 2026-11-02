# Giappone 2026 – app di viaggio

Sito mobile-first (PWA): itinerario giorno per giorno, luoghi con indirizzo e link a Google Maps,
documenti e foto (biglietti), checklist. Nessun server: dati e file restano **sul telefono**
(localStorage + IndexedDB) e funzionano anche offline dopo la prima apertura.

## Pubblicazione su GitHub Pages
1. Crea un repository su github.com (es. `giappone-trip`).
2. Nella cartella del progetto:
   ```
   git init
   git add .
   git commit -m "Prima versione"
   git branch -M main
   git remote add origin https://github.com/Pertezen/giappone-trip.git
   git push -u origin main
   ```
3. Su GitHub: Settings → Pages → Source: *Deploy from a branch* → Branch `main`, cartella `/ (root)` → Save.
4. Dopo 1–2 minuti il sito è su `https://pertezen.github.io/giappone-trip/`.

## Sul telefono
- Apri il link, poi "Aggiungi a Home" (Safari: Condividi → Aggiungi a Home; Chrome: menu → Installa app).
- Apri l'app una volta con la rete: da quel momento funziona anche offline.
- Carica i documenti **dallo stesso telefono** che userai in viaggio: i file sono salvati solo lì.

## Note
- I dati sono per dispositivo: telefono e PC non si sincronizzano. Usa "Esporta/Importa itinerario" in Info per spostare l'itinerario (i documenti non sono inclusi).
- Il sito è pubblico: non scrivere nel codice dati sensibili (numeri di prenotazione, passaporto). Quelli inseriscili dall'app, restano sul telefono.
- Per aggiornare dopo una modifica: `git add . && git commit -m "Modifica" && git push`.
