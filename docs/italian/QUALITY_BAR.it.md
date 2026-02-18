# 🏆 Quality Bar & Standard di Validazione

Per trasformare **Antigravity Awesome Skills** da una collezione di script in una piattaforma affidabile, ogni skill deve soddisfare uno specifico standard di qualità e sicurezza.

## Il Badge "Validated" ✅

Una skill ottiene il badge "Validated" solo se supera questi **5 controlli automatizzati**:

### 1. Integrità dei Metadati

Il frontmatter di `SKILL.md` deve essere un YAML valido e contenere:

- `name`: Formato kebab-case, deve corrispondere al nome della cartella.
- `description`: Sotto i 200 caratteri, con una chiara proposta di valore.
- `risk`: Uno tra `[none, safe, critical, offensive]`.
- `source`: URL alla fonte originale (o "self" se originale).

### 2. Trigger Chiari ("Quando usare")

La skill DEVE avere una sezione che indichi esplicitamente quando attivarla.

- **Esempio Positivo**: "Usa quando l'utente chiede di debuggare un componente React."
- **Esempio Negativo**: "Questa skill ti aiuta con il codice."
Intestazioni accettate: `## Quando Usare`, `## Usa questa skill quando`, `## Quando Usare Questa Skill`.

### 3. Classificazione di Sicurezza e Rischio

Ogni skill deve dichiarare il proprio livello di rischio:

- 🟢 **none**: Puro testo/ragionamento (es. Brainstorming).
- 🔵 **safe**: Legge file, esegue comandi sicuri (es. Linter).
- 🟠 **critical**: Modifica lo stato, elimina file, effettua push in produzione (es. Git Push).
- 🔴 **offensive**: Strumenti di Pentesting/Red Team. **DEVE** avere l'avviso "Solo per Uso Autorizzato".

### 4. Esempi Copia-Incolla

Almeno un blocco di codice o un esempio di interazione che un utente (o un agente) possa utilizzare immediatamente.

### 5. Limitazioni Esplicite

Un elenco di casi limite noti o cose che la skill _non_ può fare.

- _Esempio_: "Non funziona su Windows senza WSL."

---

## Livelli di Supporto

Categorizziamo le skill anche in base a chi le mantiene:

| Livello        | Badge | Significato                                         |
| :------------- | :---- | :-------------------------------------------------- |
| **Official**   | 🟣    | Gestita dal team core. Alta affidabilità.          |
| **Community**  | ⚪    | Contribuita dall'ecosistema. Supporto best effort. |
| **Verified**   | ✨    | Skill della community che ha superato una revisione manuale approfondita. |

---

## Come Validare la tua Skill

Il validatore canonico è `scripts/validate_skills.py`. Esegui `npm run validate` (o `npm run validate:strict`) prima di inviare una PR:

```bash
npm run validate       # modalità soft (solo avvertimenti)
npm run validate:strict  # modalità strict (usata dalla CI)
```
