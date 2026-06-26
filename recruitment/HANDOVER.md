# HANDOVER — Network & Systems Engineer search (Four Minds client)

**From:** Cloud session `claude/network-engineer-recruitment-wj1y7p`
**To:** Local Claude Code session (laptop, with real env / connected integrations)
**Date:** 2026-06-25
**Owner:** Joseph Marsden (James Marsden = Apollo account holder)

---

## 0. Why this handover exists
The cloud sandbox had **only Apollo (read-only), Notion (plan-gated), and GitHub** connected, with locked-down network egress. Recruitly, "turnover", Teams/Outlook, and Apollo write/credits were **not reachable** from it. The local session has the real env files and connected tools, so it can finish what the sandbox could only stage. **First job locally: fill in `.env.example` → `.env` and confirm each integration before acting.**

---

## 1. Objective
Fill the **Network Systems Engineer** role for client **Four Minds**. Find someone **like Cedric Desens but better**. Source → message → **book Teams screening calls into Joseph's diary, 09:00–11:00 tomorrow**.

## 2. Ideal candidate profile (hard bar)
- **10+ years** experience
- Strong across **ALL domains: network + security + systems** (not a specialist silo)
- **Routing & switching**
- **Ansible** (automation)
- **Proxmox** preferred (VMware or Nutanix acceptable)
- **Linux**, production/critical environments
- **Hands-on ENGINEER, not an architect**

## 3. Benchmark & existing pipeline (DEDUPE AGAINST THESE)
- **Cedric Desens** — the benchmark. Target = "better than Cedric."
- **Matthias** — in process
- **Salman Hetana** — in process
- **2 further candidates** already submitted, **not yet pushed to customer**
- These live in **Recruitly** — pull them via the Recruitly API and **exclude from any new outreach**. They were NOT found in Apollo contacts.

## 4. Operating constraints (Joseph's rules — non-negotiable)
- **No client name** ("Four Minds") in any outreach or job post
- **No TJM / day rate** disclosed in outreach or ad
- **Create urgency** — interviews tomorrow morning, slots going fast
- **Only exceptional candidates** (strong on BOTH quality AND availability/speed)
- **Don't burn all turnover credits** — up to ~100 is fine, but **add everyone contacted into the system**
- **Two-lens / XYZ check before every decision** (see §8)
- Bottom line: **book the meetings**

## 5. Shortlist (sourced from Apollo, Paris, 10+ yrs — see shortlist.csv for IDs)
Last names masked by Apollo until enriched. Enrich via `apollo_people_bulk_match` (1 credit each).

**Tier 1 — true network+security+systems breadth, hands-on IC:**
| Apollo ID | First | Title | Employer | Note |
|---|---|---|---|---|
| 54a4bb4c7468693b8c72e95e | Benoit | Senior Linux Systems & Network Engineer \| Security & Critical Env | AQSACOM | Bullseye |
| 60d0893a648bc500018c0f4a | David | Senior Systems and Network Engineer | Enix | Proxmox/Ansible near-certain |
| 5e82ebc74834c30001946f61 | Louis | Senior Network, Systems & Infrastructure Engineer | Ozitem | Multi-domain ESN |
| 54a23e2a7468693825305d19 | Kevin | Tech Lead Network Automation & Infrastructure Eng | Worldline | Automation=Ansible |
| 54a49577746869367630d752 | Andy | Lead Infrastructure Engineer | Leboncoin | Scale Linux/Proxmox |

**Tier 2 — strong network+security, confirm systems on call:**
| Apollo ID | First | Title | Employer |
|---|---|---|---|
| 54a895867468692d1c098a01 | Eric | Senior Network & Security Engineer | Cour des comptes |
| 57ded84fa6da987b015dfde1 | Naoufal | Senior Network & Security Engineer | Eutelsat |
| 55dc5794f3e5bb7918001c56 | David | Senior Network/Security Engineer | BNP Paribas AM |
| 57db79b6a6da98687b458f15 | Younes | Senior Network & Security Engineer | Butagaz |
| 57d5dd65a6da9853a66b6de3 | Mohamed | Senior Infrastructure Engineer | Exegy |

Pool size for the base query: **294** Paris matches (room to expand). Apollo search **cannot filter on Ansible/Proxmox** (keyword field indexes names/titles/employers only) — ranking used title breadth + employer type; confirm stack on the call.

## 6. Assets already produced (in this folder, committed)
- `outreach_messages.md` — FR/EN cold outreach + follow-up + slot-lock (anonymised, urgency baked in)
- `job_post.md` — job post for turnover/Recruitly (client anonymised, no TJM)
- `meetings_2026-06-26.ics` — 4 × 30-min interview HOLDS, 09:00–11:00 Europe/Paris

## 7. What the local session must verify/connect (see `.env.example`)
1. **Recruitly** — API key + base URL; confirm reachable. Use to: pull existing pipeline (dedupe), post job, add candidates, message.
2. **turnover** — CONFIRM what this platform actually is (URL/login) + whether it has an API. Post job + message.
3. **Microsoft Graph (Teams/Outlook)** — token/app reg to **write calendar events** into Joseph's diary, or generate Teams meeting links.
4. **Apollo** — needs **lead credits topped up** (was 0) AND a **linked sending mailbox** (none linked) to enrich + send sequences.
5. **Notion** — needs Business plan + Notion AI to query, IF the pipeline is mirrored there.

## 8. Two-lens (XYZ) decision check — apply before each go/no-go
- **Lens A — Quality/fit:** multi-domain (net+sec+sys), Ansible, Proxmox, hands-on IC, 10+ yrs.
- **Lens B — Conversion/speed:** reachable now, plausibly open, can take a Teams call tomorrow AM.
- **"Exceptional" = strong on BOTH.** Only those get outreach. Tier 1 qualifies first.

## 9. Local runbook (the loop, once integrations are green)
1. Fill `.env`, confirm Recruitly + Graph + Apollo (credits + mailbox) respond.
2. Recruitly: pull pipeline → build exclude-list (Cedric, Matthias, Salman, +2).
3. Apollo: enrich Tier 1 (5 credits) → real emails/dials → **add as contacts ("system")**.
4. Post `job_post.md` to turnover + Recruitly.
5. Send `outreach_messages.md` (FR) to Tier 1 via chosen channel — urgency, no client name, no TJM.
6. As replies land → create confirmed Teams invites into the 09:00–11:00 holds (Graph) → send candidate the link + slot-lock message.
7. Follow-up message at 24h to non-responders. Expand to Tier 2 / deeper pool if <4 booked.
8. Log everyone contacted into the system. Re-run the two-lens check before pushing anyone to the customer.
