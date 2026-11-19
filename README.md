# Mars Colony — Template

The planning documents behind **Mars Colony**, a real-time isometric colony simulator set on Mars. You keep a settlement alive by balancing oxygen, power and food, putting colonists to work, mining ore, and running rovers, all against a simulation that runs on the server. The 3D edition draws everything with procedural Three.js models.

There is **no code here**. These are the docs the original was built from, so you can build your own version.

## What's inside

| File | What it is |
|---|---|
| [`CONTRACT.md`](CONTRACT.md) | The full spec: data ownership, simulation rules, state shape, game pieces and their states |
| [`DESIGN.md`](DESIGN.md) | The telemetry design system: colour, typography, layout, depth and shapes |
| [`DATABASE.md`](DATABASE.md) | The database rules: namespacing, access, how the simulation runs, migrations and schema |
| [`AGENTS.md`](AGENTS.md) | The working guide for an AI coding agent: stack, conventions, and the "never do" rules that keep the simulation honest |
| [`PLAYTEST_PLAN.md`](PLAYTEST_PLAN.md) | Playtest scenarios, from oxygen starvation to offline catch-up, each saying what must happen |
| [`.agents/`](.agents) | Agent rules, a playtest workflow, and two skills (`playtest`, `long-run-player`) for testing the game with an AI agent |
| [`REFERENCE.md`](REFERENCE.md) | The original project's README: a full tour of the finished game, its mechanics, architecture and setup |

## How to use it

1. Use this template (or clone it) to start a new repo.
2. Read `CONTRACT.md` first. It's the checklist the build is held to. Change it on purpose if you want a different game.
3. Adjust `DESIGN.md` for your own look, and `DATABASE.md` if your data model changes.
4. Open the folder in Claude Code (or another agent) and build it up in stages: the simulation tick first, then rendering, then UI, then hazards and logistics. Use the playtest skills to check each stage.

Stack the docs assume: TypeScript, Vite, Three.js, Supabase (PostgreSQL, auth, edge functions), deployed on Vercel.
