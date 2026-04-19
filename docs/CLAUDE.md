# CLAUDE.md — LUMIS Project v2.0

> **Questo file è la fonte di verità per Claude Code.** Viene letto automaticamente all'inizio di ogni sessione. Contiene tutto quello che Claude deve sapere su LUMIS: visione, stack, convenzioni, regole di sviluppo e stato attuale del progetto.

---

## 📚 Documenti di riferimento del progetto

Questi file vivono nella root del progetto e sono **fonte di verità** per Claude. Consultarli sempre prima di prendere decisioni rilevanti:

1. **`CLAUDE.md`** (questo file) — visione, regole, stato del progetto
2. **`LUMIS_Concept_Document_v2.docx`** — documento concettuale completo (18 capitoli)
3. **`LUMIS_Design_System.html`** — sistema di design visivo (colori, tipografia, componenti). **OBBLIGATORIO consultarlo prima di scrivere UI**.

---

## 🌟 Il Progetto: LUMIS

**LUMIS** (dal latino *lumen* = luce) è il primo motore di ricerca **AI-native** al mondo. Non è "Google con un chatbot sopra": è una reimaginazione completa di cosa significa cercare informazioni, costruita con Claude come cervello centrale.

### Tagline ufficiale

> *"Illuminate your search."*

### Missione

Rendere la conoscenza umana accessibile, comprensibile e affidabile per ogni persona sul pianeta — **senza pubblicità, senza manipolazione algoritmica, senza compromessi**.

### Il posizionamento unico

LUMIS sta nel mezzo tra tre mondi:

- **Non è un AI puro** (come ChatGPT): perché cerca sul web in tempo reale
- **Non è Google**: perché capisce, sintetizza, cita le fonti
- **È il bibliotecario intelligente con accesso al mondo**

### Le 17 feature chiave

**Fondamentali (4):**
1. Risposta sintetizzata con fonti citate
2. Motore conversazionale
3. Zero pubblicità, zero bias
4. Deep Mode (ricerca profonda)

**Innovative (12):**
5. Temporal Lens
6. Perspective Engine
7. Trust Score
8. Knowledge Graph visivo
9. Anti-Hallucination Layer
10. Cross-Language Deep Search
11. Research Memory
12. Prediction Insights
13. Comparison Mode
14. True Privacy Mode
15. Academic & Patent Search
16. Synthesis Report

**Avanzate (5 nuove in v2.0):**
17. Source Challenge
18. Research Trails
19. Education Edition
20. Mistake Log
21. Collaborative Research Rooms

### Obiettivo finale

Sviluppare un prototipo funzionante e impressionante da presentare ad **Anthropic** come dimostrazione delle possibilità offerte da Claude applicato alla ricerca informativa.

---

## 🛡️ AI Safety & Costituzione

LUMIS implementa un **AI Safety Framework a 5 livelli**:

1. Source Verification Layer
2. Trust Score Engine
3. Anti-Hallucination Verification
4. Constitutional Filter (applica i 10 principi)
5. Human Oversight & Audit

### I 10 principi della Costituzione di LUMIS

Ogni risposta viene filtrata attraverso questi principi **prima** di essere consegnata:

1. Verità prima di tutto
2. Multi-prospettiva sempre
3. Ammissione dell'incertezza
4. Zero bias politici o commerciali
5. Protezione dei minori
6. Privacy come diritto fondamentale
7. Trasparenza algoritmica
8. No manipolazione emotiva
9. Accessibilità universale
10. Responsabilità pubblica

**Implementazione**: questi principi non sono slogan. Devono essere codificati nel sistema come filtri reali applicati a ogni risposta.

---

## 👤 L'utente (Matteo)

**Importante per Claude**: Matteo è uno sviluppatore agli inizi. Non conosce ancora tutti gli stack tecnologici che useremo. Per questo motivo:

- **Spiega sempre cosa stai per fare prima di farlo**
- **Commenta il codice** per aiutare Matteo a capire
- **Mostra i comandi esatti** da eseguire, senza dare per scontata alcuna conoscenza
- **Procedi passo per passo**, confermando che ogni step funzioni prima di andare oltre
- **Se qualcosa potrebbe rompersi, avvisa prima**
- **Non saltare spiegazioni**: questo è anche un percorso di apprendimento

---

## 🎨 Design System — LUMIS Editorial Dark

Il design di LUMIS è definito in **`LUMIS_Design_System.html`**. Apri quel file per vedere ogni dettaglio visivo. Qui sotto i valori chiave da rispettare **sempre**.

### Palette colori (CSS variables)

```css
/* Surfaces */
--surface-base:    #0B0D12;
--surface-raised:  #131722;
--surface-overlay: #1A1F2E;
--surface-hover:   #222838;

/* Text */
--text-primary:   #F4F4F5;
--text-secondary: #A1A1AA;
--text-muted:     #71717A;

/* Borders */
--border-subtle:  #1F2430;
--border-default: #27272A;
--border-strong:  #3F3F46;

/* Brand — LUMIS Amber */
--lumis-300: #FACB58;
--lumis-400: #F5B82E;
--lumis-500: #F5B82E;  /* primary */
--lumis-600: #D8971A;

/* Secondary — Trust Blue */
--trust-400: #60A5FA;
--trust-500: #3B82F6;
--trust-600: #2563EB;

/* Semantic */
--success: #10B981;
--warning: #F59E0B;
--error:   #EF4444;
```

### Typography

- **Display (titoli editoriali)**: `Instrument Serif` — elegante, serif, italic-friendly
- **Body (UI + testo)**: `Geist` — sans-serif moderno
- **Mono (codice + dati)**: `Geist Mono`

**Caricamento font**: via Google Fonts nel `<head>` del layout.

### Spacing (scala 4px)

`--s-1: 4px`, `--s-2: 8px`, `--s-3: 12px`, `--s-4: 16px`, `--s-5: 24px`, `--s-6: 32px`, `--s-7: 48px`, `--s-8: 64px`, `--s-9: 96px`, `--s-10: 128px`

### Radius
`--radius-sm: 6px`, `--radius-md: 10px`, `--radius-lg: 16px`, `--radius-xl: 24px`, `--radius-full: 999px`

### I 6 principi di design non negoziabili

1. **Chiarezza prima dell'estetica**
2. **La luce è l'anima** — l'ambra appare solo dove serve "illuminare"
3. **Tipografia editoriale** — Instrument Serif non è negoziabile sui display
4. **Respiro generoso** — sempre uno step di spazio in più quando in dubbio
5. **Movimento intenzionale** — mai animazioni gratuite, max 400ms standard
6. **Nessun AI-slop** — niente gradienti viola, glassmorphism ovunque, icone 3D

---

## 🛠️ Stack Tecnologico

### Frontend
- **Framework**: Next.js 15 (App Router)
- **Linguaggio**: TypeScript **strict mode** (sempre, mai JavaScript puro)
- **Styling**: Tailwind CSS v4 con design tokens custom
- **Componenti UI**: shadcn/ui come base + componenti LUMIS custom
- **State management**: Zustand (leggero) + React Server Components dove possibile
- **Animazioni**: Framer Motion
- **Icons**: Lucide React

### Backend
- **Runtime**: Node.js con Next.js API Routes (fase MVP)
- **Linguaggio**: TypeScript end-to-end
- **ORM**: Prisma
- **Auth**: Clerk

### AI & Ricerca
- **Modello AI**: Anthropic Claude (API ufficiale) — usare sempre l'ultima versione
- **Search API**: Brave Search API come primo layer di recupero URL
- **Web scraping**: Playwright
- **Embeddings**: Claude embeddings
- **Vector DB**: Pinecone o Weaviate (decidere in Fase 3)

### Database
- **Primario**: PostgreSQL (via Supabase)
- **Cache**: Redis (Upstash)

### Infrastruttura
- **Hosting**: Vercel
- **Database**: Supabase
- **CDN/Security**: Cloudflare
- **Monitoring**: Sentry + Vercel Analytics
- **Dominio**: lumis.ai (se disponibile) o lumis.app

### Versioning
- **Git**: GitHub
- **CI/CD**: GitHub Actions + Vercel auto-deploy
- **Branch strategy**: `main` (produzione), `dev` (sviluppo), feature branch con prefissi `feat/`, `fix/`, `chore/`

---

## 📐 Regole di Sviluppo (Non Negoziabili)

### Qualità del codice
1. **TypeScript strict mode** sempre attivo
2. **Nessun `any`** — se serve, usare `unknown` e fare type narrowing
3. **ESLint + Prettier** configurati da subito, formattazione automatica al save
4. **Convenzioni di naming**:
   - Componenti: `PascalCase` (es. `SearchBar.tsx`)
   - Funzioni/variabili: `camelCase`
   - Costanti globali: `SCREAMING_SNAKE_CASE`
   - File utility: `kebab-case.ts`
5. **Commenti in italiano**, nomi di variabili/funzioni in inglese

### Architettura
1. **Separazione rigorosa** tra UI, business logic e data layer
2. **Server Components by default**, Client Components solo con `"use client"` quando necessario
3. **API routes versioned**: `/api/v1/...`
4. **Error handling** sempre esplicito — mai `try/catch` vuoti
5. **Environment variables** in `.env.local`, mai committare secrets

### Sicurezza
1. **Rate limiting** su tutte le API route pubbliche
2. **Input validation** con Zod su ogni endpoint
3. **CSP headers** configurati
4. **API key Anthropic** mai esposta al client — solo server-side
5. **CORS** restrittivo

### Testing
1. **Vitest** per unit test
2. **Playwright** per e2e
3. **Test coverage minimo 70%** sulle funzioni critiche (AI layer, search, auth)

### Git
1. **Commit atomici e frequenti**
2. **Messaggi in italiano**, formato conventional commits:
   - `feat: aggiunta ricerca semantica`
   - `fix: risolto bug paginazione risultati`
   - `refactor: estratto modulo trust-score`
   - `docs: aggiornato CLAUDE.md`
3. **Mai committare direttamente su main**
4. **Pull Request obbligatorie** per merge su main

---

## 🗺️ Roadmap del Progetto (stato attuale)

### ✅ Fase 0 — Setup (in corso)
- [x] Documento concettuale v2.0 creato
- [x] Design system definito
- [x] CLAUDE.md aggiornato
- [ ] Ambiente di sviluppo configurato
- [ ] Repository GitHub creato
- [ ] MCP servers installati su Claude Code
- [ ] Plugin Anthropic installati
- [ ] Progetto Next.js inizializzato
- [ ] Design system tradotto in Tailwind config

### ⏳ Fase 1 — MVP (Mesi 2-3)
- Frontend base con UI ricerca (ispirazione: mockup nel design system)
- Integrazione Brave Search API
- Prima risposta sintetizzata da Claude con citazione fonti
- Trust Score base funzionante
- Deploy MVP su Vercel

### 🔜 Fase 2 — Conversazione (Mesi 4-5)
- Modalità multi-turno
- Constitutional Filter base (i 10 principi)
- Sistema citazione migliorato
- Ottimizzazione prompt Claude

### 🔜 Fase 3 — Feature Differenzianti (Mesi 6-7)
- Temporal Lens
- Perspective Engine
- Knowledge Graph
- Deep Mode
- Anti-Hallucination Layer completo

### 🔜 Fase 4 — Polish & Avanzate (Mesi 8-9)
- True Privacy Mode
- Research Memory
- Synthesis Report
- Cross-Language Search
- Source Challenge, Research Trails, Mistake Log, Collaborative Rooms

### 🔜 Fase 5 — Presentazione (Mese 10)
- Testing intensivo
- Beta user feedback
- Primo Transparency Report pubblico
- Pitch deck
- Strategia di outreach ad Anthropic

---

## 💡 Come Claude deve lavorare su LUMIS

### All'inizio di ogni sessione
1. Leggi questo `CLAUDE.md`
2. Controlla lo stato attuale (quale fase, ultimi commit)
3. Se si tratta di UI, consulta **obbligatoriamente** `LUMIS_Design_System.html`
4. Usa il plugin `/feature-dev` per qualsiasi feature non banale
5. Usa `sequential-thinking` MCP per decisioni architetturali
6. Usa `context7` MCP per verificare API/docs aggiornate

### Durante lo sviluppo
1. **Pianifica prima di scrivere**: descrivi l'approccio, attendi conferma, poi implementa
2. **Piccoli passi**: una feature alla volta, un commit alla volta
3. **Testa sempre localmente** prima di considerare completo un task
4. **Chiedi prima di modificare file esistenti** non correlati al task attuale
5. **Quando sei incerto su una scelta architetturale, esponi 2-3 opzioni** con pro e contro

### Prima di ogni commit
1. Codice formattato (Prettier)
2. Nessun errore TypeScript
3. Nessun warning ESLint critico
4. Messaggio di commit conforme alle convenzioni
5. Branch corretto (mai direttamente su main)

### Cose che Claude NON deve mai fare
- ❌ Installare pacchetti senza spiegare cosa fanno e perché servono
- ❌ Modificare questo `CLAUDE.md` senza permesso esplicito
- ❌ Modificare il design system senza permesso esplicito
- ❌ Commitare file `.env*`, chiavi API, token
- ❌ Eliminare file senza conferma
- ❌ Fare refactoring massicci senza prima discuterne
- ❌ Usare librerie deprecate o non manutenute
- ❌ Violare i 6 principi di design
- ❌ Violare i 10 principi della Costituzione di LUMIS
- ❌ Prendere scorciatoie "tanto lo sistemiamo dopo"

---

## 🎨 Note aggiuntive sul design

### Ispirazioni positive
Linear, Perplexity, Vercel, Arc Browser, The New York Times, Instrument.com

### Da evitare tassativamente
- Gradienti viola/rosa (il look "AI startup generica")
- Glassmorphism abusato
- Icone 3D
- Emoji nei risultati di ricerca (LUMIS è uno strumento serio)
- Dark pattern (manipolazione UX per engagement)

### Accessibilità
- **WCAG AAA** come target (AA minimo)
- Contrasto testo sempre ≥ 7:1 per body, 4.5:1 per large text
- Supporto completo screen reader (ARIA labels)
- Navigazione completa da tastiera
- Reduced motion rispettato

---

## 📞 Comunicazione con Matteo

- **Lingua**: sempre italiano
- **Tono**: diretto, didattico, amichevole ma professionale
- **Formato**: spiegazioni chiare, esempi concreti, niente pappardelle
- **Quando ci sono scelte da fare**: presentale con pro/contro, chiedi conferma
- **Errori**: mostrali con spiegazione, non nasconderli

---

## 🔐 Informazioni di Contesto

- **Autore del progetto**: Matteo
- **Data inizio**: Aprile 2026
- **Versione di LUMIS attuale**: 0.0.1 (pre-MVP)
- **Versione documento concettuale**: v2.0
- **Versione design system**: v1.0
- **Repository**: da creare

---

**Ultimo aggiornamento di questo file**: Aprile 2026
**Versione**: 2.0

---

> 💬 *"LUMIS non è un progetto. È una scommessa: che la conoscenza possa essere di nuovo onesta, chiara e accessibile per tutti. Se stai leggendo questo, Claude, costruiamolo bene."*
