# Guida Rapida Visuale

**Impara guardando!** Questa guida utilizza diagrammi ed esempi visivi per aiutarti a comprendere le skill.

---

## Il Quadro Generale

```
┌─────────────────────────────────────────────────────────────┐
│                    TU (Sviluppatore)                        │
│                          ↓                                  │
│              "Aiutami a costruire un sistema di pagamenti"  │
│                          ↓                                  │
│              AGENTE AI                                      │
│                          ↓                                  │
│              Carica la skill @stripe-integration            │
│                          ↓                                  │
│         Diventa un esperto nei pagamenti Stripe             │
│                          ↓                                  │
│    Fornisce aiuto specializzato con esempi di codice        │
└─────────────────────────────────────────────────────────────┘
```

---

## 📦 Struttura del Repository (Visuale)

```
antigravity-awesome-skills/
│
├── 📄 README.md                    ← Panoramica e lista delle skill
├── 📄 CONTRIBUTING.it.md           ← Come contribuire
│
├── 📁 skills/                      ← Qui vivono tutte le oltre 250 skill
│   │
│   ├── 📁 brainstorming/
│   │   └── 📄 SKILL.md             ← Definizione della skill
│   │
│   ├── 📁 stripe-integration/
│   │   ├── 📄 SKILL.md
│   │   └── 📁 examples/            ← Extra opzionali
│   │
│   └── ... (oltre 250 altre skill)
│
├── 📁 scripts/                     ← Validazione e gestione
│   ├── validate_skills.py          ← Il "guardiano" della Quality Bar
│   └── generate_index.py           ← Generatore del Registro
│
├── 📁 .github/
│   └── 📄 MAINTENANCE.md           ← Guida per i manutentori
│
└── 📁 docs/                        ← Documentazione
    ├── 📄 GETTING_STARTED.it.md    ← Inizia qui!
    ├── 📄 FAQ.it.md                ← Risoluzione dei problemi
    ├── 📄 BUNDLES.it.md            ← Starter Pack (Bundle)
    ├── 📄 QUALITY_BAR.it.md        ← Standard di Qualità
    ├── 📄 SKILL_ANATOMY.it.md      ← Come funzionano le skill
    └── 📄 VISUAL_GUIDE.it.md       ← Questo file!
```

---

## Come Funzionano le Skill (Diagramma di Flusso)

```
┌──────────────┐
│ 1. INSTALLA  │  Copia le skill in .agent/skills/
└──────┬───────┘
       │
       ↓
┌──────────────┐
│ 2. INVOCA    │  Digita: @nome-skill nella chat AI
└──────┬───────┘
       │
       ↓
┌──────────────┐
│ 3. CARICA    │  L'AI legge il file SKILL.md
└──────┬───────┘
       │
       ↓
┌──────────────┐
│ 4. ESEGUI    │  L'AI segue le istruzioni della skill
└──────┬───────┘
       │
       ↓
┌──────────────┐
│ 5. RISULTATO │  Ottieni aiuto specializzato!
└──────────────┘
```

---

## 🎯 Categorie delle Skill (Mappa Visiva)

```
                    ┌──────────────────────────────────┐
                    │   OLTRE 250 FANTASTICHE SKILL    │
                    └────────────┬─────────────────────┘
                                 │
        ┌────────────────────────┼────────────────────────┐
        │                        │                        │
   ┌────▼────┐            ┌──────▼──────┐         ┌──────▼──────┐
   │ CREATIVO│            │  SVILUPPO   │         │ SICUREZZA   │
   │ (10)    │            │    (25)     │         │    (50)     │
   └────┬────┘            └──────┬──────┘         └──────┬──────┘
        │                        │                        │
   • UI/UX Design          • TDD                    • Ethical Hacking
   • Canvas Art            • Debugging              • Metasploit
   • Temi                  • Pattern React          • Burp Suite
                                                    • SQLMap
        │                        │                        │
        └────────────────────────┼────────────────────────┘
                                 │
        ┌────────────────────────┼────────────────────────┐
        │                        │                        │
   ┌────▼────┐            ┌──────▼──────┐         ┌──────▼──────┐
   │   AI    │            │  DOCUMENTI  │         │  MARKETING  │
   │  (30)   │            │     (4)     │         │    (23)     │
   └────┬────┘            └──────┬──────┘         └──────┬──────┘
        │                        │                        │
   • Sistemi RAG           • DOCX                   • SEO
   • LangGraph             • PDF                    • Copywriting
   • Prompt Eng.           • PPTX                   • CRO
   • Agenti Vocali         • XLSX                   • Ads a pagamento
```

---

## Anatomia di un File Skill (Visuale)

````
┌─────────────────────────────────────────────────────────┐
│ SKILL.md                                                │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  ┌───────────────────────────────────────────────┐     │
│  │ FRONTMATTER (Metadati)                        │     │
│  │ ───────────────────────────────────────────── │     │
│  │ ---                                           │     │
│  │ name: mia-skill                               │     │
│  │ description: "Cosa fa questa skill"           │     │
│  │ ---                                           │     │
│  └───────────────────────────────────────────────┘     │
│                                                         │
│  ┌───────────────────────────────────────────────┐     │
│  │ CONTENUTO (Istruzioni)                         │     │
│  │ ───────────────────────────────────────────── │     │
│  │                                               │     │
│  │ # Titolo della Skill                          │     │
│  │                                               │     │
│  │ ## Panoramica                                 │     │
│  │ Cosa fa questa skill...                       │     │
│  │                                               │     │
│  │ ## Quando Usarla                              │     │
│  │ - Usa quando...                               │     │
│  │                                               │     │
│  │ ## Istruzioni                                 │     │
│  │ 1. Primo passo...                             │     │
│  │ 2. Secondo passo...                           │     │
│  │                                               │     │
│  │ ## Esempi                                     │     │
│  │ ```javascript                                 │     │
│  │ // Codice di esempio                          │     │
│  │ ```                                           │     │
│  │                                               │     │
│  └───────────────────────────────────────────────┘     │
│                                                         │
└─────────────────────────────────────────────────────────┘
````

---

## Installazione (Passaggi Visivi)

### Passo 1: Clona il Repository

```
┌─────────────────────────────────────────┐
│ Terminale                               │
├─────────────────────────────────────────┤
│ $ git clone https://github.com/        │
│   sickn33/antigravity-awesome-skills    │
│   .agent/skills                         │
│                                         │
│ ✓ Clonazione in '.agent/skills'...     │
│ ✓ Fatto!                                │
└─────────────────────────────────────────┘
```

### Passo 2: Verifica l'Installazione

```
┌─────────────────────────────────────────┐
│ Esplora File                            │
├─────────────────────────────────────────┤
│ 📁 .agent/                              │
│   └── 📁 skills/                        │
│       ├── 📁 brainstorming/             │
│       ├── 📁 stripe-integration/        │
│       ├── 📁 react-best-practices/      │
│       └── ... (altre 176)               │
└─────────────────────────────────────────┘
```

### Passo 3: Usa una Skill

```
┌─────────────────────────────────────────┐
│ Chat Assistente AI                      │
├─────────────────────────────────────────┤
│ Tu: @brainstorming aiutami a progettare │
│     una todo app                        │
│                                         │
│ AI: Ottimo! Lascia che ti aiuti a       │
│     rifletterci. Innanzitutto, capiamo   │
│     i tuoi requisiti...                 │
│                                         │
│     Qual è il caso d'uso principale?    │
│     a) Gestione task personale          │
│     b) Collaborazione di team           │
│     c) Pianificazione progetto          │
└─────────────────────────────────────────┘
```

---

## Esempio: Utilizzare una Skill (Passo dopo Passo)

### Scenario: Vuoi aggiungere i pagamenti Stripe alla tua app

```
┌─────────────────────────────────────────────────────────────┐
│ PASSO 1: Identifica il Bisogno                              │
├─────────────────────────────────────────────────────────────┤
│ "Devo aggiungere la gestione dei pagamenti alla mia app"    │
└─────────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────────┐
│ PASSO 2: Trova la Skill Giusta                              │
├─────────────────────────────────────────────────────────────┤
│ Cerca: "payment" o "stripe"                                 │
│ Trovata: @stripe-integration                                │
└─────────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────────┐
│ PASSO 3: Invoca la Skill                                    │
├─────────────────────────────────────────────────────────────┤
│ Tu: @stripe-integration aiutami ad aggiungere abbonamenti   │
└─────────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────────┐
│ PASSO 4: L'AI Carica la Skill Conoscenza                    │
├─────────────────────────────────────────────────────────────┤
│ • Pattern API Stripe                                        │
│ • Gestione Webhook                                          │
│ • Gestione Abbonamenti                                      │
│ • Migliori Pratiche                                         │
└─────────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────────┐
│ PASSO 5: Ottieni Aiuto Esperto                              │
├─────────────────────────────────────────────────────────────┤
│ L'AI fornisce:                                              │
│ • Esempi di codice                                          │
│ • Istruzioni di configurazione                              │
│ • Considerazioni sulla sicurezza                            │
│ • Strategie di testing                                      │
└─────────────────────────────────────────────────────────────┘
```

---

## Trovare le Skill (Guida Visiva)

### Metodo 1: Sfoglia per Categoria

```
README.md → Scorri fino a "Full Skill Registry" → Trova categoria → Scegli skill
```

### Metodo 2: Cerca per Parola Chiave

```
Terminale → ls skills/ | grep "parola-chiave" → Visualizza skill corrispondenti
```

### Metodo 3: Usa l'Indice

```
Apri skills_index.json → Cerca parola chiave → Trova percorso della skill
```

---

## Creare la Tua Prima Skill (Workflow Visivo)

```
┌──────────────┐
│ 1. IDEA      │  "Voglio condividere la mia conoscenza di Docker"
└──────┬───────┘
       │
       ↓
┌──────────────┐
│ 2. CREA      │  mkdir skills/docker-mastery
└──────┬───────┘  touch skills/docker-mastery/SKILL.md
       │
       ↓
┌──────────────┐
│ 3. SCRIVI    │  Aggiungi frontmatter + contenuto
└──────┬───────┘  (Usa il template da CONTRIBUTING.it.md)
       │
       ↓
┌──────────────┐
│ 4. TESTA     │  Copia in .agent/skills/
└──────┬───────┘  Prova: @docker-mastery
       │
       ↓
┌──────────────┐
│ 5. VALIDA    │  python3 scripts/validate_skills.py
└──────┬───────┘
       │
       ↓
┌──────────────┐
│ 6. INVIA     │  git commit + push + Pull Request
└──────────────┘
```

---

## Livelli di Complessità della Skill

```
┌─────────────────────────────────────────────────────────────┐
│                    COMPLESSITÀ DELLA SKILL                  │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  SEMPLICE                  STANDARD              COMPLESSA  │
│  ────────                  ────────              ─────────  │
│                                                             │
│  • 1 file                  • 1 file              • Multi-file│
│  • 100-200 parole          • 300-800 parole      • 800-2000 │
│  • Struttura base          • Struttura completa  • Script    │
│  • Nessun extra            • Esempi              • Esempi    │
│                            • Migliori pratiche   • Template  │
│                                                  • Documenti │
│  Esempio:                  Esempio:              Esempio:   │
│  git-pushing               brainstorming         loki-mode  │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## 🎯 Impatto del Contributo (Visuale)

```
Il Tuo Contributo
       │
       ├─→ Migliora la Documentazione
       │        │
       │        └─→ Aiuta migliaia di sviluppatori a capire
       │
       ├─→ Crea Nuove Skill
       │        │
       │        └─→ Abilita nuove capacità per tutti
       │
       ├─→ Corregge Bug/Errori
       │        │
       │        └─→ Previene confusione per i futuri utenti
       │
       └─→ Aggiunge Esempi
                │
                └─→ Rende l'apprendimento facile per i principianti
```

---

## Percorso di Apprendimento (Roadmap Visiva)

```
INIZIA QUI
    │
    ↓
┌───────────────────────┐
│ Leggi                 │
│ GETTING_STARTED.it.md │
└────────┬──────────────┘
         │
         ↓
┌───────────────────────┐
│ Prova 2-3 Skill       │
│ nell'assistente AI    │
└────────┬──────────────┘
         │
         ↓
┌───────────────────────┐
│ Leggi                 │
│ SKILL_ANATOMY.it.md   │
└────────┬──────────────┘
         │
         ↓
┌───────────────────────┐
│ Studia le             │
│ Skill Esistenti       │
└────────┬──────────────┘
         │
         ↓
┌───────────────────────┐
│ Crea una              │
│ Skill Semplice        │
└────────┬──────────────┘
         │
         ↓
┌───────────────────────┐
│ Leggi                 │
│ CONTRIBUTING.it.md    │
└────────┬──────────────┘
         │
         ↓
┌───────────────────────┐
│ Invia un PR           │
└────────┬──────────────┘
         │
         ↓
    CONTRIBUTORE! 🎉
```

---

## 💡 Consigli Rapidi (Cheat Sheet Visivo)

```
┌─────────────────────────────────────────────────────────────┐
│                    RIFERIMENTO RAPIDO                       │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  📥 INSTALLAZIONE                                           │
│  git clone [repo] .agent/skills                             │
│                                                             │
│  🎯 UTILIZZO                                                │
│  @nome-skill [la tua richiesta]                             │
│                                                             │
│  🔍 RICERCA                                                 │
│  ls skills/ | grep "parola-chiave"                           │
│                                                             │
│  ✅ VALIDAZIONE                                             │
│  python3 scripts/validate_skills.py                         │
│                                                             │
│  📝 CREAZIONE                                               │
│  1. mkdir skills/mia-skill                                  │
│  2. Crea SKILL.md con frontmatter                           │
│  3. Aggiungi il contenuto                                   │
│  4. Testa e valida                                          │
│  5. Invia PR                                                │
│                                                             │
│  🆘 AIUTO                                                   │
│  • docs/GETTING_STARTED.it.md - Basi                        │
│  • CONTRIBUTING.it.md - Come contribuire                    │
│  • SKILL_ANATOMY.it.md - Approfondimento                    │
│  • GitHub Issues - Fai domande                               │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## Storie di Successo (Timeline Visiva)

```
Giorno 1: Installa le skill
  │
  └─→ "Wow, @brainstorming mi ha aiutato a progettare la mia app!"

Giorno 3: Usa 5 skill diverse
  │
  └─→ "Queste skill mi fanno risparmiare un sacco di tempo!"

Settimana 1: Crea la prima skill
  │
  └─→ "Ho condiviso la mia esperienza come skill!"

Settimana 2: La skill viene approvata (merged)
  │
  └─→ "La mia skill sta aiutando gli altri! 🎉"

Mese 1: Contributore regolare
  │
  └─→ "Ho contribuito con 5 skill e migliorato i documenti!"
```

---

## Prossimi Passi

1. ✅ **Comprendi** la struttura visiva
2. ✅ **Installa** le skill nel tuo strumento AI
3. ✅ **Prova** 2-3 skill da diverse categorie
4. ✅ **Leggi** CONTRIBUTING.it.md
5. ✅ **Crea** la tua prima skill
6. ✅ **Condividi** con la community

---

**Apprendimento visivo?** Questa guida dovrebbe aiutarti! Hai ancora domande? Controlla:

- [GETTING_STARTED.it.md](GETTING_STARTED.it.md) - Introduzione testuale
- [SKILL_ANATOMY.it.md](SKILL_ANATOMY.it.md) - Analisi dettagliata
- [CONTRIBUTING.it.md](../italian/CONTRIBUTING.it.md) - Come contribuire

**Pronto a contribuire?** Ci sei quasi! 💪
