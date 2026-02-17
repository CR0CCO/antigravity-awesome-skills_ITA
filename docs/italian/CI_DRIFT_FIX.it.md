# Guida per la Risoluzione del CI Drift

**Problema**: Il fallimento del job è causato da modifiche non committate rilevate in `README.md`, `skills_index.json` o nei file del catalogo dopo l'esecuzione degli script di aggiornamento.

**Errore**:

```
❌ Detected uncommitted changes produced by registry/readme/catalog scripts.
```

**Causa**:
Script come `scripts/generate_index.py`, `scripts/update_readme.py` e `scripts/build-catalog.js` modificano `README.md`, `skills_index.json`, `data/catalog.json`, `data/bundles.json`, `data/aliases.json` e `CATALOG.md`. Il workflow si aspetta che questi file non subiscano modifiche dopo l'esecuzione degli script. Qualsiasi differenza significa che il repository committato è fuori sincronia (out-of-sync) con quanto prodotto dagli script di generazione.

**Come Risolvere (DA FARE OGNI VOLTA):**

1. Esegui la **Catena di Validazione COMPLETA** localmente:

   ```bash
   npm run chain
   npm run catalog
   ```

2. Controlla le modifiche:

   ```bash
   git status
   git diff
   ```

3. Committa e spingi (push) eventuali aggiornamenti:
   ```bash
   git add README.md skills_index.json data/catalog.json data/bundles.json data/aliases.json CATALOG.md
   git commit -m "chore: sync generated registry files"
   git push
   ```

**Sommario**:
Committa e spingi sempre tutte le modifiche prodotte dagli script del registro, del readme e del catalogo. Questo mantiene il workflow del CI funzionante assicurando che il repository e i file generati siano sincronizzati.
