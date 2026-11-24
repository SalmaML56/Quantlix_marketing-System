# One-Person Marketing Team

AI agents that run research, content, creative, posting, email, leads, website and analytics as one loop. **No post goes live until the owner approves it.**

Channels in version 1: Instagram, LinkedIn, TikTok, X (Twitter), Facebook, YouTube, plus email and the website.

## Phase status

| Phase | Name | Branch | Status | Milestone |
|---|---|---|---|---|
| 0 | Discovery, Access and Risk | `phase/00-discovery` | Not started |  |
| 1 | Foundation: Repo, Config, Database, CI | `phase/01-foundation` | Not started |  |
| 2 | Knowledge Layer (26 files) | `phase/02-knowledge-layer` | Not started |  |
| 3 | Signals and System of Record (Integrations) | `phase/03-signals-and-record` | Not started |  |
| 4 | The Brain: Runtime, Triage, Checker, Budget Guard | `phase/04-brain` | Not started |  |
| 5 | Approval Gate, Owner Controls and Interrupts | `phase/05-approval-gate` | Not started | Safe base ready |
| 6 | Research and Content Team and Competitor Watch | `phase/06-research-content` | Not started |  |
| 7 | Creative Studio and Approval Desk | `phase/07-creative-studio` | Not started |  |
| 8 | Distribution and Community | `phase/08-distribution` | Not started | First visible demo |
| 9 | Leads and Booking | `phase/09-leads-booking` | Not started |  |
| 10 | Email and Nurture | `phase/10-email-nurture` | Not started |  |
| 11 | Search and Website | `phase/11-search-website` | Not started |  |
| 12 | Analytics Loop, Observability and Morning Page | `phase/12-analytics-loop` | Not started | Full loop works |
| 13 | Hardening, Compliance and Go-Live | `phase/13-hardening-golive` | Not started | Go-live |

Status values: Not started, In progress, In review, Merged.

## Branches

- `main`: stable and approved. Updated only by a Pull Request from `develop`, approved by the reviewer, at milestones.
- `develop`: all code comes from here.
- `phase/NN-name`: one branch per phase, made from `develop`. Each phase ends with a Pull Request into `develop`, reviewed by the manager.

## Safety defaults

`DRY_RUN=true` and `PUBLISH_ENABLED=false` until the Phase 13 sign-off. Only `server/publish/gateway.py` can publish anything.
