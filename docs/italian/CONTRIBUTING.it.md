# 🤝 Guida al Contributo - V4 Enterprise Edition

**Grazie per voler migliorare questo repository!** Questa guida ti mostrerà esattamente come contribuire, anche se sei nuovo nel mondo dell'open source.
Con la versione V4, abbiamo alzato lo standard della qualità. Ti preghiamo di leggere attentamente i **nuovi Standard di Qualità** di seguito.

---

## 🧐 La "Quality Bar" (Standard V4)

**Fondamentale per le nuove skill:** Ogni skill inviata deve superare il nostro **Controllo Qualità in 5 Punti** (vedi `docs/QUALITY_BAR.md` per i dettagli):

1.  **Metadati**: Frontmatter corretto (`name`, `description`).
2.  **Sicurezza**: Nessun comando pericoloso senza etichette di "Rischio".
3.  **Chiarezza**: Chiara sezione "Quando usare".
4.  **Esempi**: Almeno un esempio di utilizzo copia-incolla.
5.  **Azioni**: Deve definire passaggi concreti, non solo "pensieri".

---

## Modi per Contribuire

Non serve essere un esperto! Ecco come chiunque può aiutare:

### 1. Migliorare la Documentazione (Il più semplice!)

- Correggere refusi o errori grammaticali
- Rendere le spiegazioni più chiare
- Aggiungere esempi alle skill esistenti
- Tradurre la documentazione in altre lingue

### 2. Segnalare Problemi

- Hai trovato qualcosa di confuso? Diccelo!
- Una skill non funziona? Faccelo sapere!
- Hai suggerimenti? Vogliamo ascoltarli!

### 3. Creare Nuove Skill

- Condividi la tua esperienza sotto forma di skill
- Colma le lacune nella collezione attuale
- Migliora le skill esistenti

### 4. Testare e Validare

- Prova le skill e segnala cosa funziona e cosa no
- Testale su diversi strumenti AI
- Suggerisci miglioramenti

---

## Configurazione per lo Sviluppo Locale

Per eseguire localmente la validazione, la generazione dell'indice e gli aggiornamenti del README:

1. **Node.js** (per il catalogo e l'installer): `npm ci`
2. **Python 3** (per gli script di validazione, indice e readme): installa le dipendenze con
   ```bash
   pip install -r requirements.txt
   ```
   Quindi puoi eseguire `npm run chain` (validazione → indice → readme) e `npm run catalog`.

**Validazione:** Il validatore canonico è **Python** (`scripts/validate_skills.py`). Usa `npm run validate` (o `npm run validate:strict` per controlli stile CI). Il validatore JavaScript (`scripts/validate-skills.js`) è legacy/opzionale e usa uno schema diverso; i controlli CI e PR si affidano solo al validatore Python.

**npm audit:** La CI esegue `npm audit --audit-level=high`. Per risolvere i problemi localmente: esegui `npm audit`, quindi `npm update` o `npm audit fix` a seconda dei casi; per modifiche radicali, aggiorna le dipendenze manualmente ed esegui i test.

---

## Come Creare una Nuova Skill

### Guida Passo-Passo

#### Passaggio 1: Scegli l'Argomento della Skill

Chiediti: "Cosa vorrei che il mio assistente AI sapesse fare meglio?".
Esempio: "Sono bravo con Docker, creerò una skill per Docker".

#### Passaggio 2: Crea la Struttura delle Cartelle

Le skill risiedono nella directory `skills/`. Usa il formato `kebab-case` per i nomi delle cartelle.

```bash
# Entra in skills
cd skills/

# Crea la cartella della tua skill
mkdir la-mia-nuova-skill
cd la-mia-nuova-skill

# Crea il file SKILL.md
touch SKILL.md
```

#### Passaggio 3: Scrivi il tuo SKILL.md

Ogni skill necessita di questa struttura di base. **Copia questo template:**

```markdown
---
name: la-mia-nuova-skill
description: "Breve descrizione di una riga su cosa fa questa skill"
---

# Titolo della Skill

## Panoramica

Spiega cosa fa questa skill e quando usarla.

## Quando Usare Questa Skill

- Usa quando [scenario 1]
- Usa quando [scenario 2]

## Come Funziona

Istruzioni dettagliate passo-passo per l'AI...

## Esempi

### Esempio 1

\`\`\`
esempio di codice qui
\`\`\`

## Migliori Pratiche

- ✅ Fai questo
- ❌ Non fare questo
```

#### Passaggio 4: Validazione (PASSAGGIO V4 CRITICO)

Usa il validatore canonico `scripts/validate_skills.py` tramite `npm run validate`. **Non approveremo PR che falliscono questo controllo.**

```bash
npm run validate        # modalità soft (solo avvertimenti)
npm run validate:strict # modalità strict (quella eseguita dalla CI)
```

Questo controlla che:

- ✅ `SKILL.md` esista
- ✅ Il Frontmatter sia corretto
- ✅ Il nome corrisponda al nome della cartella
- ✅ I controlli della Quality Bar siano superati

#### Passaggio 5: Invia la tua Skill

```bash
git add skills/la-mia-nuova-skill/
git commit -m "feat: add la-mia-nuova-skill"
git push origin mia-branch
```

---

## Template Skill (Copia & Incolla)

Risparmia tempo! Copia questo template:

```markdown
---
name: nome-della-tua-skill
description: "Una frase che descrive cosa fa questa skill e quando usarla"
---

# Nome della Tua Skill

## Panoramica

[2-3 frasi che spiegano cosa fa questa skill]

## Quando Usare Questa Skill

- Usa quando devi [scenario 1]
- Usa quando vuoi [scenario 2]

## Guida Passo-Passo

### 1. [Nome Primo Passaggio]

[Istruzioni dettagliate]

## Esempi

### Esempio 1: [Nome Caso d'Uso]

\`\`\`language
// Esempio di codice qui
\`\`\`

## Migliori Pratiche

- ✅ **Fai:** [Buona pratica]
- ❌ **Non fare:** [Cosa evitare]

## Risoluzione dei Problemi

**Problema:** [Problema Comune]
**Soluzione:** [Come risolverlo]
```

---

## Linee Guida per i Messaggi di Commit

Usa questi prefissi:

- `feat:` - Nuova skill o funzionalità principale
- `docs:` - Miglioramenti alla documentazione
- `fix:` - Correzione di bug
- `refactor:` - Miglioramenti al codice senza cambiare funzionalità
- `test:` - Aggiunta o aggiornamento di test
- `chore:` - Attività di manutenzione

**Esempi:**

```
feat: add kubernetes-deployment skill
docs: improve getting started guide
fix: correct typo in stripe-integration skill
```

---

## Risorse per l'Apprendimento

### Nuovo su Git/GitHub?

- [Guida Hello World di GitHub](https://guides.github.com/activities/hello-world/)
- [Basi di Git](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)

### Nuovo sul Markdown?

- [Guida al Markdown](https://www.markdownguide.org/basic-syntax/)

---

## Codice di Condotta

- Essere rispettosi e inclusivi
- Dare il benvenuto ai nuovi arrivati
- Concentrarsi su feedback costruttivi
- **Nessun contenuto dannoso**: Vedi `docs/SECURITY_GUARDRAILS.md`.

---

**Grazie per rendere questo progetto migliore per tutti!**
Ogni contributo, non importa quanto piccolo, fa la differenza. Che tu corregga un refuso, migliori una frase o crei una nuova skill - stai aiutando migliaia di sviluppatori!
