# Workflow di Antigravity

> Manuali di workflow per orchestrare più skill con meno attrito.

## Cos'è un Workflow?

Un workflow è un percorso di esecuzione guidato, passo dopo passo, che combina più skill per un risultato concreto.

- **I Bundle** ti dicono quali skill sono rilevanti per un ruolo.
- **I Workflow** ti dicono come usare quelle skill in sequenza per completare un obiettivo reale.

Se i bundle sono la tua cassetta degli attrezzi, i workflow sono il tuo manuale di esecuzione.

---

## Come Usare i Workflow

1. Installa il repository una volta (`npx antigravity-awesome-skills`).
2. Scegli un workflow corrispondente al tuo obiettivo immediato.
3. Esegui i passaggi in ordine e invoca le skill elencate in ogni passaggio.
4. Conserva gli artefatti prodotti in ogni fase (piano, decisioni, test, prove di validazione).

Puoi combinare i workflow con i bundle da [BUNDLES.it.md](BUNDLES.it.md) quando hai bisogno di una copertura più ampia.

---

## Workflow: Lanciare un MVP SaaS

Costruisci e lancia un prodotto SaaS minimo ma orientato alla produzione.

**Bundle correlati:** `Essentials`, `Full-Stack Developer`, `QA & Testing`, `DevOps & Cloud`

### Prerequisiti

- Repository locale e runtime configurati.
- Problema dell'utente e ambito (scope) dell'MVP chiari.
- Target di distribuzione (deployment) di base selezionato.

### Passaggi

1. **Pianifica l'ambito (scope)**
   - **Obiettivo:** Definire i confini dell'MVP e i criteri di accettazione.
   - **Skill:** [`@brainstorming`](../skills/brainstorming/), [`@concise-planning`](../skills/concise-planning/), [`@writing-plans`](../skills/writing-plans/)
   - **Esempio di prompt:** `Usa @concise-planning per definire milestone e criteri di accettazione del mio MVP SaaS.`

2. **Costruisci il backend e le API**
   - **Obiettivo:** Implementare le entità core, le API e la base dell'autenticazione.
   - **Skill:** [`@backend-dev-guidelines`](../skills/backend-dev-guidelines/), [`@api-patterns`](../skills/api-patterns/), [`@database-design`](../skills/database-design/)
   - **Esempio di prompt:** `Usa @backend-dev-guidelines per creare API e servizi del dominio billing.`

3. **Costruisci il frontend**
   - **Obiettivo:** Lanciare il flusso utente principale con stati UX chiari.
   - **Skill:** [`@frontend-developer`](../skills/frontend-developer/), [`@react-patterns`](../skills/react-patterns/), [`@frontend-design`](../skills/frontend-design/)
   - **Esempio di prompt:** `Usa @frontend-developer per implementare onboarding, empty state e dashboard iniziale.`

4. **Testa e valida**
   - **Obiettivo:** Coprire i percorsi utente critici prima del rilascio.
   - **Skill:** [`@test-driven-development`](../skills/test-driven-development/), [`@browser-automation`](../skills/browser-automation/), `@go-playwright` (opzionale, stack Go)
   - **Esempio di prompt:** `Usa @browser-automation per creare test E2E sui flussi signup e checkout.`
   - **Nota su Go:** Se il progetto QA e il tooling sono in Go, preferisci `@go-playwright`.

5. **Rilascia in sicurezza**
   - **Obiettivo:** Rilasciare con osservabilità e piano di rollback.
   - **Skill:** [`@deployment-procedures`](../skills/deployment-procedures/), [`@observability-engineer`](../skills/observability-engineer/)
   - **Esempio di prompt:** `Usa @deployment-procedures per una checklist di rilascio con rollback.`

---

## Workflow: Audit di Sicurezza per una Web App

Esegui una revisione della sicurezza mirata, dalla definizione dell'ambito alla validazione della risoluzione.

**Bundle correlati:** `Security Engineer`, `Security Developer`, `Observability & Monitoring`

### Prerequisiti

- Autorizzazione esplicita per i test.
- Target nell'ambito (in-scope) documentati.
- Dettagli di logging e dell'ambiente disponibili.

### Passaggi

1. **Definisci l'ambito e il threat model**
   - **Obiettivo:** Identificare asset, confini di fiducia (trust boundaries) e percorsi di attacco.
   - **Skill:** [`@ethical-hacking-methodology`](../skills/ethical-hacking-methodology/), [`@threat-modeling-expert`](../skills/threat-modeling-expert/), [`@attack-tree-construction`](../skills/attack-tree-construction/)
   - **Esempio di prompt:** `Usa @threat-modeling-expert per mappare asset critici e confini di fiducia (trust boundaries) della mia web app.`

2. **Rivedi l'autenticazione e il controllo degli accessi**
   - **Obiettivo:** Rilevare difetti di acquisizione account (takeover) e di autorizzazione.
   - **Skill:** [`@broken-authentication`](../skills/broken-authentication/), [`@auth-implementation-patterns`](../skills/auth-implementation-patterns/), [`@idor-testing`](../skills/idor-testing/)
   - **Esempio di prompt:** `Usa @idor-testing per verificare accessi non autorizzati su endpoint multitenant.`

3. **Valuta la sicurezza delle API e degli input**
   - **Obiettivo:** Scoprire vulnerabilità API e injection ad alto impatto.
   - **Skill:** [`@api-security-best-practices`](../skills/api-security-best-practices/), [`@api-fuzzing-bug-bounty`](../skills/api-fuzzing-bug-bounty/), [`@top-web-vulnerabilities`](../skills/top-web-vulnerabilities/)
   - **Esempio di prompt:** `Usa @api-security-best-practices per audit endpoint auth, billing e admin.`

4. **Proteggi (harden) e verifica**
   - **Obiettivo:** Trasformare i risultati in correzioni e verificare le prove della mitigazione.
   - **Skill:** [`@security-auditor`](../skills/security-auditor/), [`@sast-configuration`](../skills/sast-configuration/), [`@verification-before-completion`](../skills/verification-before-completion/)
   - **Esempio di prompt:** `Usa @verification-before-completion per provare che le mitigazioni sono effettive.`

---

## Workflow: Costruire un Sistema di Agenti AI

Progetta e consegna un agente di livello produttivo con affidabilità misurabile.

**Bundle correlati:** `Agent Architect`, `LLM Application Developer`, `Data Engineering`

### Prerequisiti

- Caso d'uso ristretto con risultati misurabili.
- Accesso ai fornitori di modelli e strumenti di osservabilità.
- Dataset iniziale o corpo di conoscenza.

### Passaggi

1. **Definisci il comportamento target e i KPI**
   - **Obiettivo:** Impostare soglie di qualità, latenza e fallimento.
   - **Skill:** [`@ai-agents-architect`](../skills/ai-agents-architect/), [`@agent-evaluation`](../skills/agent-evaluation/), [`@product-manager-toolkit`](../skills/product-manager-toolkit/)
   - **Esempio di prompt:** `Usa @agent-evaluation per definire benchmark e criteri di successo del mio agente.`

2. **Progetta il recupero (retrieval) e la memoria**
   - **Obiettivo:** Costruire un'architettura di recupero e contesto affidabile.
   - **Skill:** [`@llm-app-patterns`](../skills/llm-app-patterns/), [`@rag-implementation`](../skills/rag-implementation/), [`@vector-database-engineer`](../skills/vector-database-engineer/)
   - **Esempio di prompt:** `Usa @rag-implementation per progettare pipeline di chunking, embedding e retrieval.`

3. **Implementa l'orchestrazione**
   - **Obiettivo:** Implementare un'orchestrazione deterministica e i confini degli strumenti.
   - **Skill:** [`@langgraph`](../skills/langgraph/), [`@mcp-builder`](../skills/mcp-builder/), [`@workflow-automation`](../skills/workflow-automation/)
   - **Esempio di prompt:** `Usa @langgraph per implementare il grafo agente con fallback e human-in-the-loop.`

4. **Valuta e itera**
   - **Obiettivo:** Migliorare i punti deboli con un ciclo strutturato.
   - **Skill:** [`@agent-evaluation`](../skills/agent-evaluation/), [`@langfuse`](../skills/langfuse/), [`@kaizen`](../skills/kaizen/)
   - **Esempio di prompt:** `Usa @kaizen per prioritizzare le correzioni sulle modalità di fallimento (failure modes) rilevate dai test.`

---

## Workflow: QA e Automazione Browser

Crea un'automazione browser resiliente con esecuzione deterministica in CI.

**Bundle correlati:** `QA & Testing`, `Full-Stack Developer`

### Prerequisiti

- Ambienti di test e credenziali stabili.
- Percorsi utente critici identificati.
- Pipeline CI disponibile.

### Passaggi

1. **Prepara la strategia di test**
   - **Obiettivo:** Definire l'ambito dei percorsi (journeys), i dati di test (fixtures) e gli ambienti di esecuzione.
   - **Skill:** [`@e2e-testing-patterns`](../skills/e2e-testing-patterns/), [`@test-driven-development`](../skills/test-driven-development/)
   - **Esempio di prompt:** `Usa @e2e-testing-patterns per definire una suite E2E minima ma ad alto impatto.`

2. **Implementa i test del browser**
   - **Obiettivo:** Costruire una copertura di test robusta con selettori stabili.
   - **Skill:** [`@browser-automation`](../skills/browser-automation/), `@go-playwright` (opzionale, stack Go)
   - **Esempio di prompt:** `Usa @go-playwright per implementare la browser automation in un progetto Go.`

3. **Triage e protezione (hardening)**
   - **Obiettivo:** Rimuovere comportamenti instabili (flaky) e garantire la ripetibilità.
   - **Skill:** [`@systematic-debugging`](../skills/systematic-debugging/), [`@test-fixing`](../skills/test-fixing/), [`@verification-before-completion`](../skills/verification-before-completion/)
   - **Esempio di prompt:** `Usa @systematic-debugging per classificare e risolvere le instabilità (flakiness) in CI.`

---

## Workflow Leggibili dalle Macchine

Per strumenti e automazione, i metadati dei workflow sono disponibili in [data/workflows.json](../data/workflows.json).
