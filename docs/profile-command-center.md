# Profile Command Center Notes

Drafted for maintaining the public GitHub profile as a compact Druid / agent-framework proof funnel.

## Pinning Suggestions

Current audit: no repositories are pinned on the profile.

Recommended pinned repositories:

1. `yyswhsccc/yyswhsccc` - profile command center.
2. A new `druid-agentic-engineering-os` repo - sanitized Druid architecture, case studies, evidence board, and roadmap.
3. A new `druid-evidence` or `druid-pr-evidence` repo - auto-updated public PR evidence snapshots and weekly dashboards.
4. `yyswhsccc/Rustchain` - useful only if the fork is kept aligned and used as a contribution/evidence bridge.
5. `yyswhsccc/mgz-pkmn` - optional because it contains a maintainer-approved external merged PR signal.
6. A stronger infra/Moodle/project repo only if it demonstrates real engineering ownership; avoid pinning random forks or learning notes.

Avoid pinning repositories that make the account look like a random fork collector unless they support the Druid / agent-framework story.

## GitHub Pages Bridge

Use the README as a 15-second proof surface. Create a GitHub Pages portfolio for the full case study:

- `/` - Yongshan + Druid hero, short proof, contact CTA.
- `/druid` - architecture, operating loop, low-touch design.
- `/week` - current weekly Druid review queue.
- `/evidence` - PR evidence board and audit timestamp.
- `/contact` - Yongshan + Weijie advisor / intro partner contact.

The existing local draft lives at:

`/Users/ssr/Documents/Codex/2026-06-02/druid-pr/druid-public-package/portfolio`

Recommended future repo:

`yyswhsccc/druid-portfolio`

## Social Preview

Use `assets/druid-social-preview.svg` as the design source for a LinkedIn/GitHub social preview.

Text direction:

- `DRUID`
- `Agentic Engineering OS for Open-Source PR Work`
- `Issue Discovery -> Risk Classification -> Patch + Tests -> Review Tracking -> Adaptive Memory`
- `Built by Yongshan Yu`

If GitHub requires PNG upload for repository social preview, export the SVG to PNG at 1200x630.

## Dynamic Components

The profile currently avoids third-party dynamic badges. That is intentional.

Allowed later, with fallback:

- GitHub Readme Stats / Top Languages cards, only below the main Druid proof and with self-hosted SVG proof above them.
- A GitHub Action that updates audit timestamp, PR counts, and `docs/evidence.md`.
- Generated `metrics.svg` committed into the repo, not loaded exclusively from a third-party service.

Avoid:

- visitor counters;
- snake animations;
- badge walls;
- fragile widgets that make the profile look broken when an external service fails.
