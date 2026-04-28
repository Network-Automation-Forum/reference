# Presentations & Podcasts

Public talks and podcast appearances about the NAF Framework. Slide decks are either stored directly in this repository or linked externally; videos and audio link to the event's or podcast's recording.

<!-- Each table is ordered newest-first by date. -->

## Presentations

| Date | Event | Title | Presenter(s) | Links |
| --- | --- | --- | --- | --- |
| 2026-04 | ITNOG 10, Bologna | The Network Automation Map | Christian Adell, Damien Garros | [PDF](presentations/itnog10-2026-network-automation-map.pdf) · [PPTX](presentations/itnog10-2026-network-automation-map.pptx) |
| 2026-04 | ESNOG 35, Madrid | NAF Framework | Pete Crocker | [PDF](presentations/esnog35-2026-naf-framework.pdf) · [PPTX](presentations/esnog35-2026-naf-framework.pptx) |
| 2026-02 | NANOG 96, San Francisco | The Network Automation Map | Wim Henderickx, Damien Garros | [PDF](presentations/nanog96-2026-network-automation-map.pdf) · [PPTX](presentations/nanog96-2026-network-automation-map.pptx) · [Video](https://www.youtube.com/watch?v=MCeDVWOrnIs) |
| 2025-11 | AUTOCON 4, Austin | NAF Framework | Dinesh Dutt, Ryan Shaw | [PDF](presentations/autocon4-2025-naf-framework.pdf) · [PPTX](presentations/autocon4-2025-naf-framework.pptx) · [Video](https://youtu.be/i1eve1uB-Rs?si=kj1BK8LqAOjSH9ym) |

## Podcasts

| Date | Podcast | Episode | Guest(s) | Link |
| --- | --- | --- | --- | --- |
| 2026-04 | Total Network Operations (Packet Pushers) | TNO060 — Think Like an Architect | Damien Garros | [Listen](https://packetpushers.net/podcasts/total-network-operations/tno060-think-like-an-architect/) |
| 2026-04 | Between 0x2 Nerds | Network Automation Framework with Dinesh Dutt | Dinesh Dutt | [Listen](https://youtu.be/0ZfcibsVHFg?si=Kqj_ITj5Bczzc0q3) |

## How to add an entry

### Presentation

1. If you have a slide deck to host in the repo, drop the file into `docs/Framework/presentations/` using the naming convention `event-year-slug.{pdf,pptx}` (e.g. `autocon3-2025-naf-stack.pdf`). External links are also fine — no file needed.
2. Add a row to the **Presentations** table, keeping it ordered newest-first by date.
3. Required fields: **Date**, **Event**, **Title**, **Presenter(s)**. Omit any optional Links field that does not apply.
4. Open a pull request.

The Links column accepts any combination of:

- `[PDF](presentations/file.pdf)` — in-repo PDF
- `[PPTX](presentations/file.pptx)` — in-repo PowerPoint
- `[Slides](https://…)` — external link to slides
- `[Video](https://…)` — recording of the talk

### Podcast

1. Add a row to the **Podcasts** table, keeping it ordered newest-first by date.
2. Required fields: **Date**, **Podcast** (the show name), **Episode** (episode title), **Guest(s)**, **Link** (where to listen/watch).
3. Open a pull request.