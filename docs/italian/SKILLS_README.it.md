# Directory delle Skill (Skills Directory)

**Benvenuti nella directory delle Skill!** Questa è la raccolta di tutte le oltre 860 skill AI specializzate.

## 🤔 Cos'è una Skill?

Le Skill sono file di istruzioni specializzate che insegnano agli assistenti AI come gestire compiti specifici. Pensa a loro come a moduli di conoscenza esperta che la tua AI può caricare su richiesta.

**Un'analogia semplice:** Proprio come puoi consultare diversi esperti (un designer, un esperto di sicurezza, un professionista del marketing), le skill permettono all'AI di diventare un esperto in vari campi esattamente quando ne hai bisogno.

---

## 📂 Struttura delle Cartelle

Ogni skill risiede nella propria cartella con la seguente struttura:

```
skills/
├── nome-della-skill/        # Cartella della singola skill
│   ├── SKILL.md             # Definizione principale della skill (Richiesto)
│   ├── scripts/             # Script di supporto (Opzionale)
│   ├── examples/            # Esempi di utilizzo (Opzionale)
│   └── resources/           # Template e risorse (Opzionale)
```

**Nota importante:** Solo il file `SKILL.md` è obbligatorio. Tutto il resto è opzionale!

---

## Come Usare le Skill

### Passaggio 1: Assicurati che le skill siano configurate
I file delle skill dovrebbero trovarsi nella tua cartella `.agent/skills/` (o `.claude/skills/`, `.gemini/skills/`, ecc.)

### Passaggio 2: Attiva una skill in una conversazione AI
Usa il simbolo `@` seguito dal nome della skill:

```
@brainstorming aiutami a progettare una app todo
```

oppure

```
@stripe-integration aggiungi la gestione dei pagamenti alla mia app
```

### Passaggio 3: L'AI diventa un esperto
L'AI carica la conoscenza di quella skill e ti aiuta con competenza specifica!

---

## Ricerca delle Skill

### Metodo 1: Sfoglia questa directory
```bash
ls skills/
```

### Metodo 2: Cerca per parola chiave
```bash
ls skills/ | grep "parola-chiave"
```

### Metodo 3: Controlla il Catalogo completo
Vedi il [Catalogo delle Skill](../../CATALOG.md) per un elenco completo di tutte le oltre 860 skill organizzate per categoria.

---

## 💡 Skill Popolari da Provare

**Per i principianti:**
- `@brainstorming` - Progetta prima di programmare
- `@systematic-debugging` - Risolvi i bug in modo metodico
- `@git-pushing` - Commit con messaggi eccellenti

**Per gli sviluppatori:**
- `@test-driven-development` - Scrivi prima i test
- `@react-best-practices` - Pattern React moderni
- `@senior-fullstack` - Sviluppo Full-stack

**Per la sicurezza:**
- `@ethical-hacking-methodology` - Fondamenti di sicurezza
- `@security-auditor` - Revisione della sicurezza del codice

---

## Crea la Tua Skill

Vuoi creare una nuova skill? Dai un'occhiata a:
1. [CONTRIBUTING.it.md](CONTRIBUTING.it.md) - Come contribuire
2. [SKILL_ANATOMY.it.md](SKILL_ANATOMY.it.md) - Guida alla struttura delle skill
3. `@skill-developer` - Usa questa skill per creare nuove skill!

---

## Documenti di Riferimento

- **[Guida Iniziale](GETTING_STARTED.it.md)** - Guida rapida per iniziare
- **[Esempi](EXAMPLES.it.md)** - Esempi di utilizzo reale
- **[FAQ](FAQ.it.md)** - Domande frequenti
- **[Guida Visuale](VISUAL_GUIDE.it.md)** - Diagrammi e flussi

---

**Serve aiuto?** Controlla le [FAQ](FAQ.it.md) o apri una issue su GitHub!
