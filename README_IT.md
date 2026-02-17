# 🌌 Antigravity Awesome Skills: oltre 860 Competenze Agentiche per Claude Code, Gemini CLI, Cursor, Copilot e Altri

> **La Collezione Definitiva di oltre 860 Competenze Agentiche Universali per Assistenti alla Codifica AI — Claude Code, Gemini CLI, Codex CLI, Antigravity IDE, GitHub Copilot, Cursor, OpenCode, AdaL**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Anthropic-purple)](https://claude.ai)
[![Gemini CLI](https://img.shields.io/badge/Gemini%20CLI-Google-blue)](https://github.com/google-gemini/gemini-cli)
[![Codex CLI](https://img.shields.io/badge/Codex%20CLI-OpenAI-green)](https://github.com/openai/codex)
[![Cursor](https://img.shields.io/badge/Cursor-AI%20IDE-orange)](https://cursor.sh)
[![Copilot](https://img.shields.io/badge/GitHub%20Copilot-VSCode-lightblue)](https://github.com/features/copilot)
[![OpenCode](https://img.shields.io/badge/OpenCode-CLI-gray)](https://github.com/opencode-ai/opencode)
[![Antigravity](https://img.shields.io/badge/Antigravity-DeepMind-red)](https://github.com/sickn33/antigravity-awesome-skills)
[![AdaL CLI](https://img.shields.io/badge/AdaL%20CLI-SylphAI-pink)](https://sylph.ai/)
[![ASK Supported](https://img.shields.io/badge/ASK-Supported-blue)](https://github.com/yeasy/ask)
[![Buy Me a Book](https://img.shields.io/badge/Buy%20me%20a-book-d13610?logo=buymeacoffee&logoColor=white)](https://buymeacoffee.com/sickn33)

Se questo progetto ti aiuta, puoi [supportarlo qui](https://buymeacoffee.com/sickn33) o semplicemente aggiungere una ⭐ al repository.

**Antigravity Awesome Skills** è una libreria curata e testata sul campo di **860 competenze agentiche ad alte prestazioni**, progettate per funzionare perfettamente con tutti i principali assistenti alla codifica AI:

- 🟣 **Claude Code** (Anthropic CLI)
- 🔵 **Gemini CLI** (Google DeepMind)
- 🟢 **Codex CLI** (OpenAI)
- 🔴 **Antigravity IDE** (Google DeepMind)
- 🩵 **GitHub Copilot** (Estensione VSCode)
- 🟠 **Cursor** (IDE nativa per l'AI)
- ⚪ **OpenCode** (CLI open source)
- 🌸 **AdaL CLI** (Agente di codifica in auto-evoluzione)

Questo repository fornisce competenze essenziali per trasformare il tuo assistente AI in una **agenzia digitale full-stack**, incluse funzionalità ufficiali di **Anthropic**, **OpenAI**, **Google**, **Microsoft**, **Supabase** e **Vercel Labs**.

## Indice

- [🚀 Nuovo qui? Inizia qui!](#nuovo-qui-inizia-qui)
- [🔌 Compatibilità e Invocazione](#compatibilità-e-invocazione)
- [🛠️ Installazione](#installazione)
- [🧯 Risoluzione dei Problemi](#risoluzione-dei-problemi)
- [🎁 Collezioni Curate (Bundle)](#collezioni-curate)
- [🧭 Workflow di Antigravity](#workflow-di-antigravity)
- [📦 Funzionalità e Categorie](#funzionalità-e-categorie)
- [📚 Sfoglia oltre 860 Competenze](#sfoglia-oltre-860-competenze)
- [🤝 Come Contribuire](#come-contribuire)
- [🤝 Community](#community)
- [☕ Supporta il Progetto](#supporta-il-progetto)
- [👥 Collaboratori e Crediti](#crediti-e-fonti)
- [👥 Collaboratori del Repo](#collaboratori-del-repo)
- [⚖️ Licenza](#licenza)
- [🌟 Storia delle Stelle](#storia-delle-stelle)
- [🏷️ Argomenti GitHub](#argomenti-github)

---

## Nuovo qui? Inizia qui!

**Benvenuto nell'edizione Workflows V5.4.0.** Questa non è solo una lista di script; è un sistema operativo completo per il tuo agente AI.

### 1. 🐣 Contesto: Cos'è questo?

**Antigravity Awesome Skills** (Versione 5.4.0) è un aggiornamento massiccio alle capacità della tua AI.

Gli agenti AI (come Claude Code, Cursor o Gemini) sono intelligenti, ma mancano di **strumenti specifici**. Non conoscono il "Protocollo di Distribuzione" della tua azienda o la sintassi specifica per "AWS CloudFormation".
Le **Competenze (Skills)** sono piccoli file markdown che insegnano loro come eseguire perfettamente questi compiti specifici, ogni volta.

### 2. ⚡️ Avvio Rapido (1 minuto)

Installa una volta; poi usa gli Starter Pack in [docs/BUNDLES.md](docs/BUNDLES.md) per concentrarti sul tuo ruolo.

1. **Installa**:

   ```bash
   # Percorso predefinito: ~/.agent/skills
   npx antigravity-awesome-skills
   ```

2. **Verifica**:

   ```bash
   test -d ~/.agent/skills && echo "Competenze installate in ~/.agent/skills"
   ```

3. **Esegui la tua prima competenza**:

   > "Usa **@brainstorming** per pianificare un MVP SaaS."

4. **Scegli un bundle**:
   - **Sviluppatore Web?** inizia con `Web Wizard`.
   - **Sicurezza?** inizia con `Security Engineer`.
   - **Uso generale?** inizia con `Essentials`.

### 3. 🧠 Come si usa

Una volta installato, chiedi pure al tuo agente in modo naturale:

> "Usa la competenza **@brainstorming** per aiutarmi a pianificare un SaaS."
> "Esegui **@lint-and-validate** su questo file."

👉 **[Leggi la Guida Completa all'Avvio](docs/GETTING_STARTED.md)**

---

## Compatibilità e Invocazione

Queste competenze seguono il formato universale **SKILL.md** e funzionano con qualsiasi assistente alla codifica AI che supporti competenze agentiche.

| Strumento       | Tipo | Esempio di Invocazione            | Percorso          |
| :-------------- | :--- | :-------------------------------- | :---------------- |
| **Claude Code** | CLI  | `>> /skill-name aiutami a...`     | `.claude/skills/` |
| **Gemini CLI**  | CLI  | `(User Prompt) Usa skill-name...` | `.gemini/skills/` |
| **Codex CLI**   | CLI  | `(User Prompt) Usa skill-name...` | `.codex/skills/`  |
| **Antigravity** | IDE  | `(Agent Mode) Usa skill...`       | `.agent/skills/`  |
| **Cursor**      | IDE  | `@skill-name (nella Chat)`        | `.cursor/skills/` |
| **Copilot**     | Ext  | `(Incolla contenuto manualmente)` | N/A               |
| **OpenCode**    | CLI  | `opencode run @skill-name`        | `.agents/skills/` |
| **AdaL CLI**    | CLI  | `(Auto) Caricamento su richiesta` | `.adal/skills/`   |

> [!TIP]
> **Percorso Universale**: Raccomandiamo di clonare in `.agent/skills/`. La maggior parte degli strumenti moderni (Antigravity, CLI recenti) cercano qui per impostazione predefinita.
> **Aggiornamento Percorso OpenCode**: il percorso di opencode è cambiato in `.agents/skills` per le competenze globali. Consulta la direttiva [Place Files](https://opencode.ai/docs/skills/#place-files) sulla documentazione di OpenCode.

> [!WARNING]
> **Utenti Windows**: questo repository utilizza **symlink** per le competenze ufficiali.
> Vedi [Risoluzione dei Problemi](#risoluzione-dei-problemi) per la correzione esatta.

---

## Installazione

Per utilizzare queste competenze con **Claude Code**, **Gemini CLI**, **Codex CLI**, **Cursor**, **Antigravity**, **OpenCode** o **AdaL**:

### Opzione A: npx (consigliata)

```bash
# Predefinito: ~/.agent/skills (universale)
npx antigravity-awesome-skills

# Cursor
npx antigravity-awesome-skills --cursor

# Claude Code
npx antigravity-awesome-skills --claude

# Gemini CLI
npx antigravity-awesome-skills --gemini

# Codex CLI
npx antigravity-awesome-skills --codex

# OpenCode
npx antigravity-awesome-skills --path .agents/skills

# Percorso personalizzato
npx antigravity-awesome-skills --path ./my-skills
```

Esegui `npx antigravity-awesome-skills --help` per tutte le opzioni. Se la directory esiste già, l'installer esegue `git pull` per aggiornare.

### Opzione B: git clone

```bash
# Universale (funziona con la maggior parte degli strumenti)
git clone https://github.com/sickn33/antigravity-awesome-skills.git .agent/skills

# Specifico per Claude Code
git clone https://github.com/sickn33/antigravity-awesome-skills.git .claude/skills

# Specifico per Gemini CLI
git clone https://github.com/sickn33/antigravity-awesome-skills.git .gemini/skills

# Specifico per Codex CLI
git clone https://github.com/sickn33/antigravity-awesome-skills.git .codex/skills

# Specifico per Cursor
git clone https://github.com/sickn33/antigravity-awesome-skills.git .cursor/skills

# Per OpenCode
git clone https://github.com/sickn33/antigravity-awesome-skills.git .agents/skills
```

---

## Risoluzione dei Problemi

### `npx antigravity-awesome-skills` restituisce 404

Usa il fallback del pacchetto GitHub:

```bash
npx github:sickn33/antigravity-awesome-skills
```

### Problemi di clonazione su Windows (symlink)

Questo repository utilizza symlink per le competenze ufficiali. Abilita la Modalità Sviluppatore o esegui Git come Amministratore, quindi clona con:

```bash
git clone -c core.symlinks=true https://github.com/sickn33/antigravity-awesome-skills.git .agent/skills
```

### Competenze installate ma non rilevate dallo strumento

Installa nel percorso specifico dello strumento (ad esempio `.claude/skills`, `.gemini/skills`, `.codex/skills`, `.cursor/skills`) o usa i flag dell'installer (`--claude`, `--gemini`, `--codex`, `--cursor`, `--path`).

### Aggiornare un'installazione esistente

```bash
git -C ~/.agent/skills pull
```

### Reinstallare da zero

```bash
rm -rf ~/.agent/skills
npx antigravity-awesome-skills
```

---

## Collezioni Curate

I **Bundle** sono gruppi curati di competenze per un ruolo o un obiettivo specifico (ad esempio: `Web Wizard`, `Security Engineer`, `OSS Maintainer`).

Ti aiutano a evitare di scegliere individualmente tra oltre 700 competenze.

Cosa sono i bundle:

- Set iniziali consigliati per workflow comuni.
- Scorciatoia per l'apprendimento e un'esecuzione più rapida.

Cosa NON sono i bundle:

- Non sono un'installazione separata.
- Non sono un preset bloccato.

Come usare i bundle:

1. Installa il repository una volta.
2. Scegli un bundle in [docs/BUNDLES.md](docs/BUNDLES.md).
3. Inizia con 3-5 competenze di quel bundle nel tuo prompt.
4. Aggiungine altre solo quando necessario.

Esempi:

- Costruire un MVP SaaS: `Essentials` + `Full-Stack Developer` + `QA & Testing`.
- Rafforzare la produzione: `Security Developer` + `DevOps & Cloud` + `Observability & Monitoring`.
- Rilasciare modifiche OSS: `Essentials` + `OSS Maintainer`.

## Workflow di Antigravity

I bundle ti aiutano a scegliere le competenze. I workflow ti aiutano a eseguirle in ordine.

- Usa i bundle quando hai bisogno di raccomandazioni curate per ruolo.
- Usa i workflow quando hai bisogno di un'esecuzione passo-passo per un obiettivo concreto.

Inizia da qui:

- [docs/WORKFLOWS.md](docs/WORKFLOWS.md): playbook leggibili per gli umani.
- [data/workflows.json](data/workflows.json): metadati dei workflow leggibili dalle macchine.

I workflow iniziali includono:

- Rilascio di un MVP SaaS
- Audit di Sicurezza per una Web App
- Costruzione di un Sistema di Agenti AI
- QA e Automazione Browser (con supporto opzionale `@go-playwright` per stack Go)

## Funzionalità e Categorie

Il repository è organizzato in domini specializzati per trasformare la tua AI in un esperto in tutto il ciclo di vita dello sviluppo software:

| Categoria      | Focus                                                 | Esempi di competenze                                                            |
| :------------- | :---------------------------------------------------- | :------------------------------------------------------------------------------ |
| Architettura   | Design di sistema, ADR, C4 e pattern scalabili        | `architecture`, `c4-context`, `senior-architect`                                |
| Business       | Crescita, prezzi, CRO, SEO e go-to-market             | `copywriting`, `pricing-strategy`, `seo-audit`                                  |
| Dati e AI      | App LLM, RAG, agenti, osservabilità, analytics        | `rag-engineer`, `prompt-engineer`, `langgraph`                                  |
| Sviluppo       | Maestria dei linguaggi, pattern framework, qualità    | `typescript-expert`, `python-patterns`, `react-patterns`                        |
| Generale       | Pianificazione, documenti, scrittura, linee guida     | `brainstorming`, `doc-coauthoring`, `writing-plans`                             |
| Infrastruttura | DevOps, cloud, serverless, deployment, CI/CD          | `docker-expert`, `aws-serverless`, `vercel-deployment`                          |
| Sicurezza      | AppSec, pentesting, analisi vulnerabilità, compliance | `api-security-best-practices`, `sql-injection-testing`, `vulnerability-scanner` |
| Testing        | TDD, test design, correzioni, workflow QA             | `test-driven-development`, `testing-patterns`, `test-fixing`                    |
| Workflow       | Automazione, orchestrazione, job, agenti              | `workflow-automation`, `inngest`, `trigger-dev`                                 |

I conteggi cambiano man mano che vengono aggiunte nuove competenze. Per l'elenco completo attuale, vedi [CATALOG.md](CATALOG.md).

## Sfoglia oltre 860 Competenze

Abbiamo spostato l'intero registro delle competenze in un catalogo dedicato per mantenere pulito questo README.

👉 **[Visualizza il Catalogo Completo delle Competenze (CATALOG.md)](CATALOG.md)**

---

## Come Contribuire

Accogliamo con piacere i contributi della community! Per aggiungere una nuova competenza:

1. Fai il **Fork** del repository.
2. **Crea una nuova directory** all'interno di `skills/` per la tua competenza.
3. **Aggiungi un `SKILL.md`** con i metadati richiesti (nome e descrizione).
4. **Esegui la validazione**: `python3 scripts/validate_skills.py`.
5. **Invia una Pull Request**.

Assicurati che la tua competenza segua le migliori pratiche di Antigravity/Claude Code.

---

## Community

- [Linee Guida della Community](docs/COMMUNITY_GUIDELINES.md)
- [Politica di Sicurezza](docs/SECURITY_GUARDRAILS.md)

---

## Supporta il Progetto

Il supporto è opzionale. Questo progetto rimane gratuito e open-source per tutti.

Se questo repository ti fa risparmiare tempo o ti aiuta a rilasciare più velocemente, puoi supportare la manutenzione continua:

- [☕ Comprami un libro su Buy Me a Coffee](https://buymeacoffee.com/sickn33)

A cosa serve il supporto:

- Curatela delle competenze, test e validazione della qualità.
- Aggiornamenti della documentazione, esempi e miglioramenti dell'onboarding.
- Selezione e revisione più rapida di problemi e PR della community.

Preferisci un supporto non finanziario:

- Aggiungi una stella al repository.
- Apri segnalazioni chiare e riproducibili.
- Invia PR (competenze, documenti, correzioni).
- Condividi il progetto con altri sviluppatori.

---

## Crediti e Fonti

Siamo nani sulle spalle di giganti.

👉 **[Visualizza il Ledger Completo delle Attribuzioni](docs/SOURCES.md)**

I principali contributori e fonti includono:

- **HackTricks**
- **OWASP**
- **Anthropic / OpenAI / Google**
- **La Community Open Source**

Questa collezione non sarebbe stata possibile senza l'incredibile lavoro della community di Claude Code e delle fonti ufficiali:

### Fonti Ufficiali

- **[anthropics/skills](https://github.com/anthropics/skills)**: Repository ufficiale delle competenze Anthropic - manipolazione documenti (DOCX, PDF, PPTX, XLSX), linee guida del marchio, comunicazioni interne.
- **[anthropics/claude-cookbooks](https://github.com/anthropics/claude-cookbooks)**: Notebook e ricette ufficiali per costruire con Claude.
- **[remotion-dev/skills](https://github.com/remotion-dev/skills)**: Competenze ufficiali Remotion - creazione video in React con 28 regole modulari.
- **[vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)**: Competenze ufficiali Vercel Labs - Migliori pratiche React, linee guida web design.
- **[openai/skills](https://github.com/openai/skills)**: Catalogo delle competenze OpenAI Codex - competenze agentiche, Skill Creator, pianificazione concisa.
- **[supabase/agent-skills](https://github.com/supabase/agent-skills)**: Competenze ufficiali Supabase - Migliori pratiche Postgres.
- **[microsoft/skills](https://github.com/microsoft/skills)**: Competenze ufficiali Microsoft - servizi cloud Azure, Bot Framework, Servizi Cognitivi e pattern di sviluppo enterprise su .NET, Python, TypeScript, Go, Rust e Java.
- **[google-gemini/gemini-skills](https://github.com/google-gemini/gemini-skills)**: Competenze ufficiali Gemini - API Gemini, SDK e interazioni con i modelli.

### Collaboratori della Community

- **[rmyndharis/antigravity-skills](https://github.com/rmyndharis/antigravity-skills)**: Per il massiccio contributo di oltre 300 competenze Enterprise e la logica di generazione del catalogo.

- **[obra/superpowers](https://github.com/obra/superpowers)**: L'originale "Superpowers" di Jesse Vincent.
- **[guanyang/antigravity-skills](https://github.com/guanyang/antigravity-skills)**: Estensioni principali di Antigravity.
- **[diet103/claude-code-infrastructure-showcase](https://github.com/diet103/claude-code-infrastructure-showcase)**: Linee guida Infrastruttura e Backend/Frontend.
- **[ChrisWiles/claude-code-showcase](https://github.com/ChrisWiles/claude-code-showcase)**: Pattern UI React e Design System.
- **[travisvn/awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills)**: Loki Mode e integrazione Playwright.
- **[zebbern/claude-code-guide](https://github.com/zebbern/claude-code-guide)**: Suite di sicurezza completa e Guida (Fonte per ~60 nuove competenze).
- **[alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills)**: Toolkit di Senior Engineering e PM.
- **[karanb192/awesome-claude-skills](https://github.com/karanb192/awesome-claude-skills)**: Una lista enorme di competenze verificate per Claude Code.
- **[VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills)**: Collezione curata di 61 competenze di alta qualità, incluse competenze ufficiali dei team di Sentry, Trail of Bits, Expo, Hugging Face e suite completa di context engineering (integrazione v4.3.0).
- **[zircote/.claude](https://github.com/zircote/.claude)**: Riferimento competenze per lo sviluppo Shopify.
- **[vibeforge1111/vibeship-spawner-skills](https://github.com/vibeforge1111/vibeship-spawner-skills)**: Agenti AI, integrazioni, strumenti per maker (57 competenze, Apache 2.0).
- **[coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)**: Competenze di marketing per CRO, copywriting, SEO, annunci a pagamento e crescita (23 competenze, MIT).
- **[vudovn/antigravity-kit](https://github.com/vudovn/antigravity-kit)**: Template per agenti AI con competenze, agenti e workflow (33 competenze, MIT).
- **[affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code)**: Collezione completa di configurazioni Claude Code dal vincitore dell'hackathon Anthropic - solo competenze (8 competenze, MIT).
- **[whatiskadudoing/fp-ts-skills](https://github.com/whatiskadudoing/fp-ts-skills)**: Competenze pratiche fp-ts per TypeScript – fp-ts-pragmatic, fp-ts-react, fp-ts-errors (v4.4.0).
- **[webzler/agentMemory](https://github.com/webzler/agentMemory)**: Fonte per la competenza agent-memory-mcp.
- **[sstklen/claude-api-cost-optimization](https://github.com/sstklen/claude-api-cost-optimization)**: Risparmia il 50-90% sui costi dell'API Claude con strategie di ottimizzazione intelligenti (MIT).
- **[Wittlesus/cursorrules-pro](https://github.com/Wittlesus/cursorrules-pro)**: Configurazioni professionali .cursorrules per 8 framework - Next.js, React, Python, Go, Rust e altri. Funziona con Cursor, Claude Code e Windsurf.

### Ispirazioni

- **[f/awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)**: Ispirazione per la libreria dei prompt.
- **[leonardomso/33-js-concepts](https://github.com/leonardomso/33-js-concepts)**: Ispirazione per la maestria di JavaScript.

---

## Collaboratori del Repo

<a href="https://github.com/sickn33/antigravity-awesome-skills/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=sickn33/antigravity-awesome-skills" />
</a>

Realizzato con [contrib.rocks](https://contrib.rocks).

Ringraziamo ufficialmente i seguenti collaboratori per il loro aiuto nel rendere questo repository fantastico!

- [@sck000](https://github.com/sck000)
- [@munir-abbasi](https://github.com/munir-abbasi)
- [@sickn33](https://github.com/sickn33)
- [@Mohammad-Faiz-Cloud-Engineer](https://github.com/Mohammad-Faiz-Cloud-Engineer)
- [@Dokhacgiakhoa](https://github.com/Dokhacgiakhoa)
- [@IanJ332](https://github.com/IanJ332)
- [@chauey](https://github.com/chauey)
- [@PabloSMD](https://github.com/PabloSMD)
- [@GuppyTheCat](https://github.com/GuppyTheCat)
- [@Tiger-Foxx](https://github.com/Tiger-Foxx)
- [@arathiesh](https://github.com/arathiesh)
- [@liyin2015](https://github.com/liyin2015)
- [@1bcMax](https://github.com/1bcMax)
- [@ALEKGG1](https://github.com/ALEKGG1)
- [@ar27111994](https://github.com/ar27111994)
- [@BenedictKing](https://github.com/BenedictKing)
- [@whatiskadudoing](https://github.com/whatiskadudoing)
- [@LocNguyenSGU](https://github.com/LocNguyenSGU)
- [@yubing744](https://github.com/yubing744)
- [@SuperJMN](https://github.com/SuperJMN)
- [@truongnmt](https://github.com/truongnmt)
- [@viktor-ferenczi](https://github.com/viktor-ferenczi)
- [@c1c3ru](https://github.com/c1c3ru)
- [@ckdwns9121](https://github.com/ckdwns9121)
- [@fbientrigo](https://github.com/fbientrigo)
- [@junited31](https://github.com/junited31)
- [@KrisnaSantosa15](https://github.com/KrisnaSantosa15)
- [@sstklen](https://github.com/sstklen)
- [@taksrules](https://github.com/taksrules)
- [@zebbern](https://github.com/zebbern)
- [@vuth-dogo](https://github.com/vuth-dogo)
- [@mvanhorn](https://github.com/mvanhorn)
- [@rookie-ricardo](https://github.com/rookie-ricardo)
- [@evandro-miguel](https://github.com/evandro-miguel)
- [@raeef1001](https://github.com/raeef1001)
- [@devchangjun](https://github.com/devchangjun)
- [@jackjin1997](https://github.com/jackjin1997)
- [@ericgandrade](https://github.com/ericgandrade)
- [@sohamganatra](https://github.com/sohamganatra)
- [@Nguyen-Van-Chan](https://github.com/Nguyen-Van-Chan)
- [@8hrsk](https://github.com/8hrsk)
- [@Wittlesus](https://github.com/Wittlesus)

---

## Licenza

Licenza MIT. Vedi [LICENSE](LICENSE) per i dettagli.

---

## Storia delle Stelle

[![Star History Chart](https://api.star-history.com/svg?repos=sickn33/antigravity-awesome-skills&type=date&legend=top-left)](https://www.star-history.com/#sickn33/antigravity-awesome-skills&type=date&legend=top-left)

Se Antigravity Awesome Skills ti è stato utile, considera di aggiungere una ⭐ stella al repo o di [comprarmi un libro](https://buymeacoffee.com/sickn33).

---

## Argomenti GitHub

Per i manutentori del repository, aggiungi questi argomenti per massimizzare la visibilità:

```text
claude-code, gemini-cli, codex-cli, antigravity, cursor, github-copilot, opencode,
agentic-skills, ai-coding, llm-tools, ai-agents, autonomous-coding, mcp,
ai-developer-tools, ai-pair-programming, vibe-coding, skill, skills, SKILL.md, rules.md, CLAUDE.md, GEMINI.md, CURSOR.md
```
