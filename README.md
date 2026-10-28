## Sebastián León

Bogotá, Colombia. Trained as a lawyer. I build tools that do the repetitive part
of people's work. That leaves them free for the decisions that need them. I keep
the tools running after they ship.

Two are used for real accounting work: one at an accounting practice, one at
client sites. Another has published a daily market report on its own since
August 2026. When I can, I compare the result with the manual work it replaced.

I start with the people and their work. What does it cost them? Where do
mistakes hide? Which decisions still need a person? I build the tool around
those answers. The two accounting tools are private, so each one has a written
case study instead.

### Selected work

[**InvestIA**](https://github.com/c0llaborative/investia) · case study
Publishes a checked daily report on 38 listings in the Colombian stock market. It has run
on its own since 26 August 2026. The hard part was trust: how do you know it is
still right when nobody is watching? It uses a second data source only to catch
the first one's mistakes. Failed checks stay in a queue until a person reviews
them.

[**legal-sparring**](https://github.com/c0llaborative/legal-sparring)
Helps a lawyer prepare for a civil hearing in Colombia. It reads the case file
and suggests the other side's likely arguments. Every point shows the page of the
file it comes from. An optional check redoes the analysis when a citation is
not backed by the file. Hackathon prototype, built with Juan Torres.

[**Causación de retenciones**](https://github.com/c0llaborative/causacion-retenciones) · case study
Used by an accounting practice since June 2026. Each month, an accountant
spent about two hours working out the tax withheld on every invoice. The tool
takes 3 to 6 minutes for about 30 invoices. Mistakes are hard to
spot, because a wrong rate still gives a believable number. This tool does the
work from the original invoices and checks each one with the tax authority,
DIAN. Compared with a month done by hand, it agreed on 93.6% of 392 data
points. The amounts withheld for all three taxes matched on every invoice. Most differences
were mistakes in the hand-made version.

[**ContaYa and SiigoYa**](https://github.com/c0llaborative/contaya-siigoya) · case study
Turned a hundred manual decisions into twelve. Recording a month of electronic
invoices went from days of an accountant's work to hours. Only a few decisions
needed the accountant. These
desktop tools do the rest, so the accountant handles only those few. In a test
run on 98 real documents, the totals matched the originals exactly. Twelve were
flagged for a person to review. Installed at client sites. Shipped
five releases between August and October 2026.

[**Contados**](https://github.com/c0llaborative/Contados)
After the 10 August 2026 earthquake, we looked for a way to check aid status by
ID number. Neither the national disaster agency (UNGRD) nor five city halls
offered one. With Contados, a family sends a WhatsApp voice note. From what the
family says, it estimates their step in the process and explains what comes
next. If it is not sure,
it asks instead of guessing. It also drafts a formal request the state must
answer within 15 business days. Hackathon prototype, tested with made-up cases
on a test WhatsApp number. Colombia Tech Week 2026, justice track.

[**crezca-landing-page**](https://github.com/c0llaborative/crezca-landing-page)
Website and waitlist for Crezca, a working financial analysis product. The
waitlist tests demand before a wider launch. If the confirmation email fails,
the signup is still saved. Next.js, TypeScript,
Supabase.

### Also on GitHub

[**pdf-legal-checker**](https://github.com/c0llaborative/pdf-legal-checker)
Checks VAWA and T-visa immigration forms for errors before they are filed. I
built it while working as a legal clerk, from the errors that kept coming back.

[**ats-harvest**](https://github.com/c0llaborative/ats-harvest)
Collects job postings from Greenhouse, Lever and Ashby into one format. Each run
says whether it finished, partly finished or failed. That way, incomplete runs
can be left out of the trends.

[**fare-watch**](https://github.com/c0llaborative/fare-watch)
Tells you when a flight price is worth buying, based on that route's past
prices. Two private copies have run on their own since July and August 2026.

[**laptop-health**](https://github.com/c0llaborative/laptop-health)
A daily health check for a Windows laptop. I wrote it after the maker's own
tool reported a fan failure that was not real. When the laptop later froze, its
logs recorded no overheating or hardware errors. That pointed to the real cause:
Windows was not allowed to use disk space as extra memory.

### Tools

Python, TypeScript, PowerShell. n8n for workflow automation. Salesforce (Litify),
used daily as a legal clerk. Browser automation, reading data from PDFs, and
scheduled jobs, with alerts when one quietly stops.

### Contact

[LinkedIn](https://www.linkedin.com/in/juan-sebastian-leon-molina/)
