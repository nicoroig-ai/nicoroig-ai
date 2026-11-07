## Nico Roig

I build systems that talk to people. Multi-tenant platforms where WhatsApp, Instagram and inbound phone calls land in one timeline, and an AI agent carries the conversation from first message to booked appointment.

Mostly TypeScript and Postgres, and a working knowledge of the parts of an integration that only break in production.

### Projects

Four systems, each written up with its architecture and the decisions behind it → **[nicoroig.dev](https://nicoroig.dev)**

| | |
|---|---|
| **AI messaging** · real estate | An assistant that answers an agency's own WhatsApp, Instagram and phone line — qualifies leads, searches their property catalogue, books viewings, follows up, hands over to a human when it should. Co-founder and technical lead; one codebase and one database serving every agency. Ran a paying client's live inbound channel in production. |
| **Purchasing** · hospitality | Predicts what a restaurant's kitchen will sell, turns that into what must be bought from each supplier before each delivery cut-off, and puts a ready-to-send order in front of the chef instead of a dashboard. Ran in production. |
| **Tax-law research** · tax & legal | A desktop tool that replaces a manual browser workflow: searches the tax authority's public rulings database, reads each ruling in full, extracts the official answer and gathers the related court criteria into a spreadsheet. Runs on a locked-down corporate machine with nothing installed and no credentials. |
| **Cognitive training** · learning | Spaced repetition and adaptive working-memory training in one app, honest about which of the two does what. Fully offline with no account; signing up later adopts the history you already have. |

### Open source

| | |
|---|---|
| **[phone-identity](https://github.com/nicoroig-ai/phone-identity)** | Canonical E.164 so the same person matches across WhatsApp, SIP and web forms. Zero dependencies. |
| **[supabase-multitenant-rls](https://github.com/nicoroig-ai/supabase-multitenant-rls)** | Pool multi-tenancy enforced by Row Level Security, with tests that try to break the isolation against a real Postgres. |
| **[meta-webhooks](https://github.com/nicoroig-ai/meta-webhooks)** | Verify and normalise WhatsApp, Instagram and Lead Ads webhooks into typed events. Runs on Node, Bun, Deno and edge runtimes. |

Each one was extracted from a platform in production, rewritten and tested on its own.

### Writing

**[architecture-notes](https://github.com/nicoroig-ai/architecture-notes)** — decisions from production systems and what they cost. The current note covers replacing a no-code stack (GoHighLevel + n8n) with a code-native multi-tenant platform: why isolation belongs in the database, why the job queue is a Postgres table rather than a workflow framework, and why a hosting constraint produced a better design than an unlimited budget would have.

### Working with

`TypeScript` · `Next.js` · `Postgres` · `Supabase` · `Vercel` · `Meta Cloud API` · `LLM orchestration` · `SIP / voice agents`

---

📫 [nicoroigmeseguer@gmail.com](mailto:nicoroigmeseguer@gmail.com) · 🌐 [nicoroig.dev](https://nicoroig.dev)
