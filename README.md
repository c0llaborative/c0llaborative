## Sebastián León

Bogotá, Colombia. Trained as a lawyer. I write the software that removes work
someone was doing by hand, and then I keep it running.

The pattern repeats across domains that have nothing to do with each other.
Someone performs a job manually, the job turns out to have rules, and the rules
can be written down and checked. Tax withholding, immigration paperwork,
securities filings and airfare all gave way to the same approach.

Several of the systems below run unattended today. Two are used by accounting
practices with paying clients, which is why their source is private and why
each has a written case study instead.

### Recent

- **2026-10-28** · Published [legal-sparring](https://github.com/c0llaborative/legal-sparring),
  a LegalTech hackathon prototype built with Juan Torres.
- **2026-10-04** · Released ContaYa and SiigoYa v1.3.6. DIAN changed its document
  search, and downloads came back empty without an error. The fix reads every
  page of results and marks a doubtful download as incomplete.
- **2026-09-17** · Causación de retenciones 1.5.0. Each company now confirms
  its own withholding criteria before any month is processed.

### Systems in use

[**Causación de retenciones**](https://github.com/c0llaborative/causacion-retenciones)
The monthly Colombian withholding-tax close, rebuilt from the source invoices.
It recomputes retefuente, ReteIVA and ICA from the 2026 rate tables and
verifies each invoice against the DIAN portal by its CUFE. Compared cell by
cell against a month a person had prepared by hand, it agreed on 93.6% of 392
field comparisons, and matched on all three withholding amounts for every
invoice. Most of the disagreements turned out to be errors in the manual paper.

[**ContaYa and SiigoYa**](https://github.com/c0llaborative/contaya-siigoya)
Desktop tools taking a month of electronic invoices from portal download to
posted accounting entries. A dry run over 98 real documents balanced to the
source XML and flagged 12 of the 98 as needing a person, which is the actual
product: a hundred manual decisions became twelve. Installed at client sites.
The latest version, v1.3.6, ships through
[public releases](https://github.com/c0llaborative/accountant-releases).

[**InvestIA**](https://github.com/c0llaborative/investia)
Publishes a validated daily report on 30 Colombian issuers. Built to fail
loudly on a thin market where a stale price and a dead feed look identical:
per-instrument staleness allowances, an independent cross-check, and a watchdog
that alerts on the run that did not happen.

### Code you can read

[**legal-sparring**](https://github.com/c0llaborative/legal-sparring)
Prepares a lawyer for a civil hearing under Colombia's Código General del
Proceso. From the case file, it rebuilds the other side's theory of the case.
Every point cites the folio of the record it rests on. Hackathon prototype,
built with Juan Torres.

[**ats-harvest**](https://github.com/c0llaborative/ats-harvest)
Reads job postings from Greenhouse, Lever and Ashby into one normalized schema.
Every run resolves to complete, partial or failed, so a source returning 3
postings instead of 300 is never read as a quiet day.

[**fare-watch**](https://github.com/c0llaborative/fare-watch)
Round-trip airfare watcher with a two-lane alert ratchet and a headless-browser
fallback for routes that only render client-side. Two private instances have
run unattended since July and August 2026.

[**laptop-health**](https://github.com/c0llaborative/laptop-health)
A daily Windows health check read straight from WMI, the event log and SMART.
Written after the vendor's own tool reported a fan failure that did not exist.
It later found a real one the vendor tool never surfaced.

[**pdf-legal-checker**](https://github.com/c0llaborative/pdf-legal-checker)
Validates VAWA and T-visa immigration forms before filing. Built while working
as a legal clerk, from the errors that kept coming back.

[**Contados**](https://github.com/c0llaborative/Contados)
Tells a displaced family over WhatsApp which stage of the aid process they are
in, what comes next, and where to do it. Colombia Tech Week 2026 hackathon,
justice track.

[**crezca-landing-page**](https://github.com/c0llaborative/crezca-landing-page)
Marketing site and waitlist for a financial analysis product. Next.js,
TypeScript, Supabase.

### Tools

Python, PowerShell, TypeScript, React. Browser automation over the Chrome
DevTools Protocol. PDF extraction and in-place PDF rewriting with PyMuPDF.
Scheduled and unattended jobs, and the monitoring that tells you when one of
them has quietly stopped.

### Contact

[LinkedIn](https://www.linkedin.com/in/juan-sebastian-leon-molina/)
