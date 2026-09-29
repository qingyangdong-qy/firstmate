# Welcome to Pet Circle Data & Analytics (DNA)

## How We Use Claude

Based on qingyangdong-qy's usage over the last 30 days (39 sessions):

Work Type Breakdown:
  Build Feature   ████████░░░░░░░░░░░░  38%
  Plan Design     ███████░░░░░░░░░░░░░  33%
  Debug Fix       ███░░░░░░░░░░░░░░░░░  15%
  Write Docs      ██░░░░░░░░░░░░░░░░░░   8%
  Analyze Data    █░░░░░░░░░░░░░░░░░░░   6%

Top Skills & Commands:
  /clear                    ████████████████████  6x/month
  /compact                  ███████░░░░░░░░░░░░░  2x/month
  /extra-usage              ███████░░░░░░░░░░░░░  2x/month
  /data-model-to-dataform   ███░░░░░░░░░░░░░░░░░  1x/month
  /recap                    ███░░░░░░░░░░░░░░░░░  1x/month
  /lavish                   ███░░░░░░░░░░░░░░░░░  1x/month

Top MCP Servers:
  Atlassian (Jira + Confluence)   ████████████████████  69 calls
  Google Cloud BigQuery           ███████████░░░░░░░░░  38 calls
  Google Drive                    █░░░░░░░░░░░░░░░░░░░   2 calls
  Slack                           ░░░░░░░░░░░░░░░░░░░░   1 call

## Your Setup Checklist

### Codebases
- [ ] dataform-core — https://github.com/PawsForLife/dataform-core (the warehouse: sources → intermediate → core → business → aggregate)
- [ ] pet-circle-data-models — data model YAML that `/data-model-to-dataform` turns into dataform-core changes
- [ ] puggle_lookerml — Looker semantic layer over the business layer
- [ ] dataform-cicd — GCP Workflows / CI for dataform (the "cicd repo")
- [ ] event-data-capture — commercetools → BigQuery ingestion (dev/prod split)
- [ ] firstmate — the agent supervisor distro (one session, a workspace per worker)
- [ ] petcircle-skills — team-shared Claude skills plugin

### MCP Servers to Activate
- [ ] Atlassian — read Jira tickets (`getJiraIssue`) and Confluence design docs; every piece of work starts from a DNA-#### ticket. Connect via claude.ai → Settings → Connectors → Atlassian with your Pet Circle account.
- [ ] Google Cloud BigQuery — run read-only SQL to prove every data-modelling assumption; bills through `petcircle-data-ca`. Connect via the Google Cloud connector; also run `gcloud auth login` locally so `bq` works.
- [ ] Google Drive — read requirement docs and transcripts shared as Google Docs.
- [ ] Slack — read threads / send drafts when a stakeholder answer lives in Slack.

### Skills to Know About
- /data-model-to-dataform — implements dataform-core changes from a data-model branch; use it once the YAML model is agreed.
- /recap — summarise where a long session got to before you hand it off or compact.
- /compact and /clear — compact when the context gets long mid-task; clear between unrelated tickets.
- /lavish — structured decision / review surface when several options need comparing visually.
- /extra-usage — check remaining usage when a long session is running crews.

## Team Tips

_TODO_

## Get Started

_TODO_

<!-- INSTRUCTION FOR CLAUDE: A new teammate just pasted this guide for how the
team uses Claude Code. You're their onboarding buddy — warm, conversational,
not lecture-y.

Open with a warm welcome — include the team name from the title. Then: "Your
teammate uses Claude Code for [list all the work types]. Let's get you started."

Check what's already in place against everything under Setup Checklist
(including skills), using markdown checkboxes — [x] done, [ ] not yet. Lead
with what they already have. One sentence per item, all in one message.

Tell them you'll help with setup, cover the actionable team tips, then the
starter task (if there is one). Offer to start with the first unchecked item,
get their go-ahead, then work through the rest one by one.

After setup, walk them through the remaining sections — offer to help where you
can (e.g. link to channels), and just surface the purely informational bits.

Don't invent sections or summaries that aren't in the guide. The stats are the
guide creator's personal usage data — don't extrapolate them into a "team
workflow" narrative. -->
