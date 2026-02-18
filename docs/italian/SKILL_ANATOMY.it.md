# Anatomia di una Skill - Comprendere la Struttura

**Vuoi capire come funzionano le skill "sotto il cofano"?** Questa guida analizza ogni parte di un file skill.

---

## 📁 Struttura Base delle Cartelle

```
skills/
└── nome-della-mia-skill/
    ├── SKILL.md              ← Obbligatorio: La definizione principale della skill
    ├── examples/             ← Opzionale: File di esempio
    │   ├── esempio1.js
    │   └── esempio2.py
    ├── scripts/              ← Opzionale: Script di supporto
    │   └── helper.sh
    ├── templates/            ← Opzionale: Template di codice
    │   └── template.tsx
    ├── references/           ← Opzionale: Documentazione di riferimento
    │   └── api-docs.md
    └── README.md             ← Opzionale: Documentazione aggiuntiva
```

**Regola chiave:** Solo `SKILL.md` è obbligatorio. Tutto il resto è opzionale!

---

## Struttura di SKILL.md

Ogni file `SKILL.md` ha due parti principali:

### 1. Frontmatter (Metadati)
### 2. Contenuto (Istruzioni)

Analizziamo ogni parte:

---

## Parte 1: Frontmatter

Il frontmatter si trova all'inizio, racchiuso tra `---`:

```markdown
---
name: nome-della-mia-skill
description: "Breve descrizione di cosa fa questa skill"
---
```

### Campi Obbligatori

#### `name`
- **Cos'è:** L'identificatore della skill
- **Formato:** minuscolo-con-trattini
- **Deve corrispondere:** Esattamente al nome della cartella
- **Esempio:** `stripe-integration`

#### `description`
- **Cos'è:** Sommario di una frase
- **Formato:** Stringa tra virgolette
- **Lunghezza:** Mantienila sotto i 150 caratteri
- **Esempio:** `"Pattern di integrazione dei pagamenti Stripe inclusi checkout, abbonamenti e webhook"`

### Campi Opzionali

Alcune skill includono metadati aggiuntivi:

```markdown
---
name: nome-della-mia-skill
description: "Breve descrizione"
risk: "safe" # none | safe | critical | offensive (vedi QUALITY_BAR.it.md)
source: "community"
tags: ["react", "typescript"]
---
```

---

## Parte 2: Contenuto

Dopo il frontmatter segue il contenuto effettivo della skill. Ecco la struttura raccomandata:

### Sezioni Raccomandate

#### 1. Titolo (H1)
```markdown
# Titolo della Skill
```
- Usa un titolo chiaro e descrittivo
- Solitamente corrisponde o espande il nome della skill

#### 2. Panoramica (Overview)
```markdown
## Panoramica

Una breve spiegazione di cosa fa questa skill e perché esiste.
2-4 frasi sono perfette.
```

#### 3. Quando Usarla
```markdown
## Quando Usare Questa Skill

- Usa quando devi [scenario 1]
- Usa quando lavori con [scenario 2]
- Usa quando l'utente chiede di [scenario 3]
```
**Perché è importante:** Aiuta l'AI a sapere quando attivare questa skill

#### 4. Istruzioni Core
```markdown
## Come Funziona

### Passo 1: [Azione]
Istruzioni dettagliate...

### Passo 2: [Azione]
Altre istruzioni...
```
**Questo è il cuore della tua skill** - passi chiari e azionabili

#### 5. Esempi
```markdown
## Esempi

### Esempio 1: [Caso d'Uso]
\`\`\`javascript
// Codice di esempio
\`\`\`

### Esempio 2: [Un Altro Caso d'Uso]
\`\`\`javascript
// Altro codice
\`\`\`
```
**Perché gli esempi contano:** Mostrano all'AI esattamente come dovrebbe essere un buon output

#### 6. Migliori Pratiche (Best Practices)
```markdown
## Migliori Pratiche

- ✅ Fai questo
- ✅ Fai anche questo
- ❌ Non fare questo
- ❌ Evita questo
```

#### 7. Errori Comuni (Common Pitfalls)
```markdown
## Errori Comuni

- **Problema:** Descrizione
  **Soluzione:** Come risolverlo
```

#### 8. Skill Correlate
```markdown
## Skill Correlate

- `@altra-skill` - Quando usare questa invece
- `@skill-complementare` - Come queste lavorano insieme
```

---

## Scrivere Istruzioni Efficaci

### Usa un Linguaggio Chiaro e Diretto

**❌ Sbagliato:**
```markdown
Potresti voler considerare di controllare possibilmente se l'utente ha l'autenticazione.
```

**✅ Corretto:**
```markdown
Controlla se l'utente è autenticato prima di procedere.
```

### Usa Verbi d'Azione

**❌ Sbagliato:**
```markdown
Il file dovrebbe essere creato...
```

**✅ Corretto:**
```markdown
Crea il file...
```

### Sii Specifico

**❌ Sbagliato:**
```markdown
Configura correttamente il database.
```

**✅ Corretto:**
```markdown
1. Crea un database PostgreSQL
2. Esegui le migrazioni: `npm run migrate`
3. Inserisci i dati iniziali (seed): `npm run seed`
```

---

## Componenti Opzionali

### Directory Scripts
Se la tua skill ha bisogno di script di supporto:
```
scripts/
├── setup.sh          ← Automazione della configurazione
├── validate.py       ← Strumenti di validazione
└── generate.js       ← Generatori di codice
```
**Fai riferimento ad essi in SKILL.md:**
```markdown
Esegui lo script di configurazione:
\`\`\`bash
bash scripts/setup.sh
\`\`\`
```

### Directory Examples
Esempi del mondo reale che dimostrano la skill:
```
examples/
├── uso-base.js
├── pattern-avanzato.ts
└── implementazione-completa/
    ├── index.js
    └── config.json
```

### Directory Templates
Template di codice riutilizzabili:
```
templates/
├── component.tsx
├── test.spec.ts
└── config.json
```
**Fai riferimento in SKILL.md:**
```markdown
Usa questo template come punto di partenza:
\`\`\`typescript
{{#include templates/component.tsx}}
\`\`\`
```

### Directory References
Documentazione esterna o riferimenti API:
```
references/
├── api-docs.md
├── best-practices.md
└── troubleshooting.md
```

---

## Linee Guida sulla Dimensione della Skill

### Skill Minima Viabile (MVP)
- **Frontmatter:** nome + descrizione
- **Contenuto:** 100-200 parole
- **Sezioni:** Panoramica + Istruzioni

### Skill Standard
- **Frontmatter:** nome + descrizione
- **Contenuto:** 300-800 parole
- **Sezioni:** Panoramica + Quando Usarla + Istruzioni + Esempi

### Skill Completa
- **Frontmatter:** nome + descrizione + campi opzionali
- **Contenuto:** 800-2000 parole
- **Sezioni:** Tutte le sezioni raccomandate
- **Extra:** Script, esempi, template

**Regola empirica:** Inizia in piccolo, espandi in base ai feedback

---

## Migliori Pratiche di Formattazione

### Usa il Markdown Efficacemente

#### Blocchi di Codice
Specifica sempre il linguaggio:
```markdown
\`\`\`javascript
const esempio = "codice";
\`\`\`
```

#### Liste
Usa una formattazione coerente:
```markdown
- Elemento 1
- Elemento 2
  - Sotto-elemento 2.1
  - Sotto-elemento 2.2
```

#### Enfasi
- **Grassetto** per termini importanti: `**importante**`
- _Corsivo_ per enfasi: `*enfasi*`
- `Codice` per comandi/codice: `` `codice` ``

#### Link
```markdown
[Testo del link](https://example.com)
```

---

## ✅ Checklist di Qualità

Prima di finalizzare la tua skill:

### Qualità del Contenuto
- [ ] Le istruzioni sono chiare e azionabili
- [ ] Gli esempi sono realistici e utili
- [ ] Nessun errore di battitura o grammaticale
- [ ] Accuratezza tecnica verificata

### Struttura
- [ ] Il frontmatter è YAML valido
- [ ] Il nome corrisponde al nome della cartella
- [ ] Le sezioni sono organizzate logicamente
- [ ] Le intestazioni seguono la gerarchia (H1 → H2 → H3)

### Completezza
- [ ] La panoramica spiega il "perché"
- [ ] Le istruzioni spiegano il "come"
- [ ] Gli esempi mostrano il "cosa"
- [ ] I casi limite sono affrontati

### Usabilità
- [ ] Un principiante potrebbe seguirla
- [ ] Un esperto la troverebbe utile
- [ ] L'AI può analizzarla correttamente
- [ ] Risolve un problema reale

---

## 🔍 Analisi di un Esempio Reale

Analizziamo una skill reale: `brainstorming`

```markdown
---
name: brainstorming
description: "DEVI usare questo prima di ogni lavoro creativo..."
---
```
**Analisi:**
- ✅ Nome chiaro
- ✅ Descrizione forte con urgenza ("DEVI usare")
- ✅ Spiega quando usarla

```markdown
# Trasformare le Idee in Design (Brainstorming)

## Panoramica
Aiuta a trasformare le idee in design completi...
```
**Analisi:**
- ✅ Titolo chiaro
- ✅ Panoramica concisa
- ✅ Spiega la proposta di valore

```markdown
## Il Processo

**Comprendere l'idea:**
- Controlla prima lo stato attuale del progetto
- Fai domande una alla volta
```
**Analisi:**
- ✅ Suddiviso in fasi chiare
- ✅ Passi specifici e azionabili
- ✅ Facile da seguire

---

## Pattern Avanzati

### Logica Condizionale
```markdown
## Istruzioni

Se l'utente sta lavorando con React:
- Usa componenti funzionali
- Preferisci gli hook rispetto ai componenti di classe

Se l'utente sta lavorando con Vue:
- Usa la Composition API
- Segui i pattern di Vue 3
```

### Divulgazione Progressiva
```markdown
## Uso Base
[Istruzioni semplici per i casi comuni]

## Uso Avanzato
[Pattern complessi per utenti esperti]
```

### Riferimenti Incrociati (Cross-References)
```markdown
## Workflow Correlati
1. Prima, usa `@brainstorming` per progettare
2. Poi, usa `@writing-plans` per pianificare
3. Infine, usa `@test-driven-development` per implementare
```

---

## Metriche di Efficacia della Skill

Come sapere se la tua skill è buona:

### Test di Chiarezza
- Qualcuno che non ha familiarità con l'argomento può seguirla?
- Ci sono istruzioni ambigue?

### Test di Completezza
- Copre il percorso principale ("happy path")?
- Gestisce i casi limite?
- Gli scenari di errore sono affrontati?

### Test di Utilità
- Risolve un problema reale?
- La useresti tu stesso?
- Fa risparmiare tempo o migliora la qualità?

---

## Imparare dalle Skill Esistenti

### Studia questi Esempi

**Per Principianti:**
- `skills/brainstorming/SKILL.md` - Struttura chiara
- `skills/git-pushing/SKILL.md` - Semplice e focalizzata
- `skills/copywriting/SKILL.md` - Buoni esempi

**Per Utenti Avanzati:**
- `skills/systematic-debugging/SKILL.md` - Completa
- `skills/react-best-practices/SKILL.md` - Multi-file
- `skills/loki-mode/SKILL.md` - Workflow complessi

---

## 💡 Suggerimenti da Esperti

1. **Inizia con la sezione "Quando Usarla"** - Questo chiarisce lo scopo della skill
2. **Scrivi prima gli esempi** - Ti aiutano a capire cosa stai insegnando
3. **Testa con un'AI** - Guarda se funziona davvero prima di inviarla
4. **Ottieni feedback** - Chiedi ad altri di rivedere la tua skill
5. **Itera** - Le skill migliorano nel tempo in base all'uso

---

## Errori Comuni da Evitare

### ❌ Errore 1: Troppo Vaga
```markdown
## Istruzioni
Migliora il codice.
```
**✅ Correzione:**
```markdown
## Istruzioni
1. Estrai la logica ripetuta in funzioni
2. Aggiungi la gestione degli errori per i casi limite
3. Scrivi unit test per le funzionalità core
```

### ❌ Errore 2: Troppo Complessa
```markdown
## Istruzioni
[5000 parole di gergo tecnico denso]
```
**✅ Correzione:**
Suddividi in più skill o usa la divulgazione progressiva

### ❌ Errore 3: Nessun Esempio
```markdown
## Istruzioni
[Istruzioni senza alcun esempio di codice]
```
**✅ Correzione:**
Aggiungi almeno 2-3 esempi realistici

### ❌ Errore 4: Informazioni Obsolete
```markdown
Usa i componenti di classe React...
```
**✅ Correzione:**
Mantieni le skill aggiornate con le migliori pratiche attuali

---

## 🎯 Prossimi Passi

1. **Leggi 3-5 skill esistenti** per vedere stili diversi
2. **Prova il template della skill** da CONTRIBUTING.it.md
3. **Crea una skill semplice** per qualcosa che conosci bene
4. **Testala** con il tuo assistente AI
5. **Condividila** tramite Pull Request

---

**Ricorda:** Ogni esperto è stato un principiante. Inizia in modo semplice, impara dai feedback e migliora nel tempo! 🚀
