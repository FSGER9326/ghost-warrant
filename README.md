# Ghost Warrant

A mobile-first, Chrome-installable cyberpunk contact-network RPG built with Phaser, TypeScript, Vite, and DOM UI. The repository is the shared source of truth for ongoing chat- and automation-driven development.

## Run locally

```bash
npm install
npm run dev
```

Open the local URL in Chrome. For a production build:

```bash
npm run build
npm run preview
```

Chrome installation requires HTTPS or localhost. Use the browser install control after the first successful load.

## Current playable systems

- Character reconstruction and background consequences
- Floodline Exchange exploration
- Eight contacts with physical and secure-network access
- Contact commerce, services, dialogue, contracts, and specialist resale
- Six parent factions and twenty-five internal subfactions
- Persistent reputation, influence, inventory, heat, quests, and autosave
- Understation 7A safehouse with medbay, signal cage, workshop, supplies, and upgrades
- Four persistent recruitable operatives with deployment, health, loyalty, stress, and wounds
- Turn-based Black Banner medical-cache encounter with movement, attacks, enemy AI, line of sight, directional cover, smoke, suppression, disruption, wounds, victory, and extraction
- Signature combat actions for the player and all four recruitable operatives
- Offline-capable Chrome PWA production build

## Controls

- Movement: WASD, arrow keys, or mobile directional pad
- Interact: E or the contextual interaction button
- Tactical combat: select a friendly unit, select a reachable tile to move, select a visible enemy in range to attack, use the HUD ability button for the selected unit's signature action, then end the crew turn

## Tactical rules

- Solid freight cells block movement and line of sight.
- Directional cover reduces incoming damage by 2, to a minimum of 1.
- Red target rings indicate exposed shots; amber rings indicate covered targets.
- Signature abilities cost 1 AP and can be used once per encounter.
- Low Tide's smoke reduces hostile damage for the current enemy phase.
- Suppression reduces hostile damage; disruption removes a hostile action.

## Testing

```bash
npm test
```

The browser test exercises character creation, safehouse travel, facilities, contacts, purchases, remote contracts, combat launch, signature abilities, line-of-sight checks, enemy turns, victory, quest progression, Mara recruitment, crew persistence, and landscape-mobile controls.


## Shared development

Read `AGENTS.md` before automated work. Current architecture and handoff state live in `docs/ARCHITECTURE.md` and `docs/DEVELOPMENT_STATE.md`. Planned milestones live in `ROADMAP.md`.

Use `agent/<description>` branches and draft pull requests for substantial work. The GitHub Actions workflow validates production builds, static smoke checks, and browser regressions.
