# 🛡️ Guardrail e Policy di Sicurezza

Antigravity Awesome Skills è un toolkit potente. Da un grande potere derivano grandi responsabilità. Questo documento definisce le **Regole di Ingaggio** per tutte le capacità di sicurezza e offensive in questo repository.

## 🔴 Policy sulle Skill Offensive (La "Linea Rossa")

**Cos'è una Skill Offensiva?**
Qualsiasi skill progettata per penetrare, sfruttare, interrompere o simulare attacchi contro i sistemi.
_Esempi: Pentesting, SQL Injection, Simulazione di Phishing, Red Teaming._

### 1. Dichiarazione di "Solo per Uso Autorizzato"

Ogni skill offensiva **DEVE** iniziare con questa esatta dichiarazione nel suo `SKILL.md`:

> **⚠️ SOLO PER USO AUTORIZZATO**
> Questa skill è solo a scopo educativo o per valutazioni di sicurezza autorizzate.
> Devi avere un permesso esplicito e scritto dal proprietario del sistema prima di utilizzare questo strumento.
> L'uso improprio di questo strumento è illegale e severamente vietato.

### 2. Conferma Obbligatoria dell'Utente

Le skill offensive non devono **MAI** essere eseguite in modo completamente autonomo.

- **Requisito**: La descrizione/istruzioni della skill devono dire esplicitamente all'agente di _chiedere la conferma dell'utente_ prima di eseguire qualsiasi comando di exploit o attacco.
- **Istruzione per l'Agente**: "Chiedi all'utente di verificare l'URL/IP di destinazione prima dell'esecuzione."

### 3. Sicuro per Progettazione (Safe by Design)

- **Nessun Payload Armato**: Le skill non devono includere malware attivo, ransomware o exploit non educativi.
- **Sandbox Consigliata**: Le istruzioni dovrebbero raccomandare l'esecuzione in un ambiente isolato (Docker/VM).

---

## 🔵 Policy sulle Skill Difensive

**Cos'è una Skill Difensiva?**
Strumenti per il rafforzamento (hardening), l'audit, il monitoraggio o la protezione dei sistemi.
_Esempi: Linting, Analisi dei Log, Audit della Configurazione._

- **Privacy dei Dati**: Le skill difensive non devono caricare dati su server di terze parti senza l'esplicito consenso dell'utente.
- **Non Distruttivo**: Gli audit dovrebbero essere di sola lettura per impostazione predefinita.

---

## ⚖️ Dichiarazione di Non Responsabilità Legale

Utilizzando questo repository, accetti che:

1. Sei responsabile delle tue azioni.
2. Gli autori e i collaboratori non sono responsabili per eventuali danni causati da questi strumenti.
3. Rispetterai tutte le leggi locali, statali e federali riguardanti la cybersicurezza.
