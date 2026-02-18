# Guida per Iniziare con Antigravity Awesome Skills (V4)

**Nuovo qui? Questa guida ti aiuterà a potenziare il tuo Agente AI in 5 minuti.**

---

## 🤔 Cosa sono le "Skill"?

Gli agenti AI (come **Claude Code**, **Gemini**, **Cursor**) sono intelligenti, ma mancano di conoscenze specifiche sui tuoi strumenti.
Le **Skill** sono manuali di istruzioni specializzati (file markdown) che insegnano alla tua AI come eseguire compiti specifici in modo perfetto, ogni volta.

**Analogia:** La tua AI è uno stagista brillante. Le **Skill** sono le SOP (Procedure Operative Standard) che lo trasformano in un Senior Engineer.

---

## ⚡️ Inizio Rapido: I "Pacchetti Starter"

Non farti prendere dal panico per le oltre 700 skill. Non ti servono tutte in una volta.
Abbiamo curato dei **Pacchetti Starter** per farti iniziare immediatamente.

**Installa l'intero repo una sola volta** (tramite npx o clone); i Pacchetti Starter sono liste curate per aiutarti a **scegliere quali skill usare** in base al tuo ruolo (es. Web Wizard, Hacker Pack) — non sono un modo diverso per installare.

### 1. Installa il Repository

**Opzione A — npx (la più semplice):**

```bash
npx antigravity-awesome-skills
```

Questo clona il repo in `~/.agent/skills` per impostazione predefinita. Usa `--cursor`, `--claude`, `--gemini` o `--codex` per installarlo per uno strumento specifico, oppure `--path <dir>` per una posizione personalizzata. Esegui `npx antigravity-awesome-skills --help` per i dettagli.

Se visualizzi un errore 404, usa: `npx github:sickn33/antigravity-awesome-skills`

**Opzione B — git clone:**

```bash
# Universale (funziona per la maggior parte degli agenti)
git clone https://github.com/sickn33/antigravity-awesome-skills.git .agent/skills
```

### 2. Scegli la Tua Persona

Trova il bundle che corrisponde al tuo ruolo (vedi [BUNDLES.it.md](BUNDLES.it.md)):

| Persona               | Nome Bundle    | Cosa c'è dentro?                                  |
| :-------------------- | :------------- | :------------------------------------------------ |
| **Sviluppatore Web**  | `Web Wizard`   | Pattern React, padronanza di Tailwind, Design FE   |
| **Security Engineer** | `Hacker Pack`  | OWASP, Metasploit, Metodologia Pentest            |
| **Manager / PM**      | `Product Pack` | Brainstorming, Planning, SEO, Strategia           |
| **Tutto**             | `Essentials`   | Codice Pulito, Pianificazione, Valutazione (Basi) |

---

## 🧭 Bundle vs Workflow

Bundle e workflow risolvono problemi diversi:

- **Bundle** = set curati per ruolo (cosa scegliere).
- **Workflow** = playbook passo-passo (come eseguire).

Inizia con i bundle in [BUNDLES.it.md](BUNDLES.it.md), poi esegui un workflow da [WORKFLOWS.md](../../WORKFLOWS.md) quando hai bisogno di un'esecuzione guidata.

Esempio:

> "Usa **@antigravity-workflows** ed esegui `ship-saas-mvp` per la mia idea di progetto."

---

## 🚀 Come Usare una Skill

Una volta installata, parla normalmente con la tua AI.

### Esempio 1: Pianificare una Funzionalità (**Essentials**)

> "Usa **@brainstorming** per aiutarmi a progettare un nuovo flusso di login."

**Cosa succede:** L'AI carica la skill di brainstorming, ti pone domande strutturate e produce una specifica professionale.

### Esempio 2: Controllare il tuo Codice (**Web Wizard**)

> "Esegui **@lint-and-validate** su questo file e correggi gli errori."

**Cosa succede:** L'AI segue regole di linting rigorose definite nella skill per pulire il tuo codice.

### Esempio 3: Audit di Sicurezza (**Hacker Pack**)

> "Usa **@api-security-best-practices** per revisionare i miei endpoint API."

**Cosa succede:** L'AI controlla il tuo codice rispetto agli standard OWASP.

---

## 🔌 Strumenti Supportati

| Strumento       | Stato             | Percorso          |
| :-------------- | :---------------- | :---------------- |
| **Claude Code** | ✅ Supporto Completo | `.claude/skills/` |
| **Gemini CLI**  | ✅ Supporto Completo | `.gemini/skills/` |
| **Codex CLI**   | ✅ Supporto Completo | `.codex/skills/`  |
| **Antigravity** | ✅ Nativo           | `.agent/skills/`  |
| **Cursor**      | ✅ Nativo           | `.cursor/skills/` |
| **Copilot**     | ⚠️ Solo Testo      | Copia-incolla manuale|

---

## 🛡️ Fiducia & Sicurezza (Novità nella V4)

Classifichiamo le skill in modo che tu sappia cosa stai eseguendo:

- 🟣 **Official**: Gestite da Anthropic/Google/Vendor (Alta Fiducia).
- 🔵 **Safe**: Skill della community non distruttive (Sola lettura/Pianificazione).
- 🔴 **Risk**: Skill che modificano il sistema o eseguono test di sicurezza (Solo Uso Autorizzato).

_Controlla il [Catalogo delle Skill](../../CATALOG.md) per l'elenco completo._

---

## ❓ FAQ

**D: Devo installare tutte le 700+ skill?**
R: Cloni l'intero repository una volta; la tua AI _legge_ solo le skill che invochi (o che sono rilevanti), quindi rimane leggera. I **Pacchetti Starter** in [BUNDLES.it.md](BUNDLES.it.md) sono liste curate per aiutarti a scoprire le skill giuste per il tuo ruolo — non cambiano il modo in cui le installi.

**D: Posso creare le mie skill?**
R: Sì! Usa la skill **@skill-creator** per creare le tue.

**D: È gratuito?**
R: Sì, Licenza MIT. Open Source per sempre.

---

## ⏭️ Prossimi Passi

1. [Sfoglia i Bundle](BUNDLES.it.md)
2. [Vedi Esempi del Mondo Reale](../../EXAMPLES.md)
3. [Contribuisci con una Skill](../CONTRIBUTING.it.md)
