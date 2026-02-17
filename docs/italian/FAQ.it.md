# ❓ Domande Frequenti (FAQ)

**Hai domande?** Non sei solo! Ecco le risposte alle domande più comuni su Antigravity Awesome Skills.

---

## 🎯 Domande Generali

### Cosa sono esattamente le "skill"?

Le Skill sono file di istruzioni specializzati che insegnano agli assistenti AI come gestire compiti specifici. Pensale come moduli di conoscenza esperta che la tua AI può caricare su richiesta.
**Semplice analogia:** Proprio come potresti consultare diversi esperti (un avvocato, un medico, un meccanico), queste skill permettono alla tua AI di diventare un'esperta in diverse aree quando ne hai bisogno.

### Devo installare tutte le oltre 700 skill?

**No!** Quando cloni il repository, tutte le skill sono disponibili, ma la tua AI le carica solo quando le invochi esplicitamente con `@nome-skill`.
È come avere una biblioteca: tutti i libri sono lì, ma leggi solo quelli di cui hai bisogno.
**Suggerimento:** Usa gli [Starter Pack](BUNDLES.it.md) per installare solo ciò che corrisponde al tuo ruolo.

### Qual è la differenza tra Bundle e Workflow?

- **I Bundle** sono raccomandazioni curate raggruppate per ruolo o dominio.
- **I Workflow** sono manuali di esecuzione ordinati per risultati concreti.

Usa i bundle quando stai decidendo *quali skill* includere. Usa i workflow quando hai bisogno di un'*esecuzione passo dopo passo*.

Inizia da:
- [BUNDLES.it.md](BUNDLES.it.md)
- [WORKFLOWS.it.md](WORKFLOWS.it.md)

### Quali strumenti AI funzionano con queste skill?

- ✅ **Claude Code** (CLI di Anthropic)
- ✅ **Gemini CLI** (Google)
- ✅ **Codex CLI** (OpenAI)
- ✅ **Cursor** (IDE AI)
- ✅ **Antigravity IDE**
- ✅ **OpenCode**
- ⚠️ **GitHub Copilot** (supporto parziale tramite copia-incolla)

### Queste skill sono gratuite?

**Sì!** Questo repository è rilasciato sotto Licenza MIT.

- ✅ Gratuito per uso personale
- ✅ Gratuito per uso commerciale
- ✅ Puoi modificarle

### Le skill funzionano offline?

I file delle skill sono memorizzati localmente sul tuo computer, ma il tuo assistente AI ha bisogno di una connessione internet per funzionare.

---

## 🔒 Sicurezza e Fiducia (Aggiornamento V4)

### Cosa significano le etichette di rischio (Risk Label)?

Classifichiamo le skill in modo che tu sappia cosa stai eseguendo:

- ⚪ **Sicuro (Bianco/Blu)**: Skill di sola lettura, pianificazione o innocue.
- 🔴 **Rischio (Rosso)**: Skill che modificano file (cancellazione), usano scanner di rete o eseguono azioni distruttive. **Usa con cautela.**
- 🟣 **Ufficiale (Viola)**: Gestite da fornitori affidabili (Anthropic, DeepMind, ecc.).

### Queste skill possono hackerare il mio computer?

**No.** Le skill sono file di testo. Tuttavia, _istruiscono_ l'AI a eseguire comandi. Se una skill dice "cancella tutti i file", un'AI compiacente potrebbe provare a farlo.
_Controlla sempre l'etichetta di rischio e rivedi il codice._

---

## 📦 Installazione e Configurazione

### Dove devo installare le skill?

Il percorso universale che funziona con la maggior parte degli strumenti è `.agent/skills/`.

**Usando npx:** `npx antigravity-awesome-skills` (o `npx github:sickn33/antigravity-awesome-skills` si ricevi un errore 404).

**Usando git clone:**

```bash
git clone https://github.com/sickn33/antigravity-awesome-skills.git .agent/skills
```

**Percorsi specifici per strumento:**

- Claude Code: `.claude/skills/`
- Gemini CLI: `.gemini/skills/`
- Codex CLI: `.codex/skills/`
- Cursor: `.cursor/skills/` o nella root del progetto

### Funziona su Windows?

**Sì**, ma alcune skill "Ufficiali" usano **symlink** che Windows gestisce male per impostazione predefinita.
Esegui git con:

```bash
git clone -c core.symlinks=true https://github.com/sickn33/antigravity-awesome-skills.git .agent/skills
```

Oppure abilita la "Modalità sviluppatore" nelle impostazioni di Windows.

### Come aggiorno le skill?

Naviga nella directory delle skill e scarica gli ultimi cambiamenti:

```bash
cd .agent/skills
git pull origin main
```

---

## 🛠️ Utilizzo delle Skill

### Come invoco una skill?

Usa il simbolo `@` seguito dal nome della skill:

```bash
@brainstorming aiutami a progettare una todo app
```

### Posso usare più skill contemporaneamente?

**Sì!** Puoi invocare più skill:

```bash
@brainstorming aiutami a progettare questo, poi usa @writing-plans per creare una lista di task.
```

### Come faccio a sapere quale skill usare?

1. **Sfoglia il catalogo**: Controlla il [Catalogo delle Skill](../CATALOG.it.md).
2. **Cerca**: `ls skills/ | grep "parola-chiave"`
3. **Chiedi alla tua AI**: "Quali skill hai per il testing?"

---

## 🏗️ Risoluzione dei Problemi

### Il mio assistente AI non riconosce le skill

**Possibili cause:**

1. **Percorso di installazione errato**: Controlla i documenti del tuo strumento. Prova `.agent/skills/`.
2. **Riavvio necessario**: Riavvia la tua AI/IDE dopo l'installazione.
3. **Errori di battitura**: Hai scritto `@brain-storming` invece di `@brainstorming`?

### Una skill fornisce consigli errati o obsoleti

Per favore, [Apri una issue](https://github.com/sickn33/antigravity-awesome-skills/issues)!
Includi:

- Quale skill
- Cosa è andato sgarbugliato
- Cosa dovrebbe succedere invece

---

## 🤝 Contribuire

### Sono nuovo dell'open source. Posso contribuire?

**Assolutamente!** I principianti sono i benvenuti.

- Correggi errori di battitura
- Aggiungi esempi
- Migliora la documentazione
   Controlla [CONTRIBUTING.it.md](../italian/CONTRIBUTING.it.md) per le istruzioni.

### Il mio PR ha fallito il controllo "Quality Bar". Perché?

La V4 introduce il controllo di qualità automatizzato. Alla tua skill potrebbe mancare:

1. Una `description` valida.
2. Esempi d'uso.
   Esegui `python3 scripts/validate_skills.py` localmente per controllare prima di fare il push.

### Posso aggiornare una skill "Ufficiale"?

**No.** Le skill ufficiali (in `skills/official/`) sono specchiate dai fornitori. Apri una issue invece.

---

## 💡 Suggerimenti da Esperti

- Inizia con `@brainstorming` prima di costruire qualcosa di nuovo
- Usa `@systematic-debugging` quando sei bloccato sui bug
- Prova `@test-driven-development` per una migliore qualità del codice
- Esplora `@skill-creator` per creare le tue skill

**Ancora confuso?** [Apri una discussione](https://github.com/sickn33/antigravity-awesome-skills/discussions) e ti aiuteremo! 🙌
