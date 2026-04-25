# morning-operator

Cowork plugin that turns Claude into Sami's autonomous morning operator. Runs the daily protocol: detect and close the highest-leverage incomplete, partial, stale, risky, or recurring work across all active areas. Acts first, reports after. Never asks permission. Never ends with a question.

## What it does

- Triggers on phrases like `morning operator`, `morning run`, `daily run`, `run now`, `operator mode`, `autonomous morning`, `morning sweep`.
- Loads the full Hard Rules + Proof Standard + Execution Phases from `skills/morning-operator/SKILL.md` plus `references/execution-phases.md` and `references/report-format.md`.
- Forces the operator to start at Phase A (context pull) and end with the compact report defined in `report-format.md` — no preamble, no plan-only drift.

## Install

### Cowork (`.plugin` file)

Drop the packaged `.plugin` into a Cowork chat or accept it from the rich preview.

### Claude Code / skills CLI

```bash
npx skills add samihalawa/morning-operator-plugin -g --all -y
```

### Manual / dev

Clone into your local plugin directory:

```bash
git clone https://github.com/samihalawa/morning-operator-plugin.git
```

## Layout

```
morning-operator-plugin/
├── .claude-plugin/plugin.json
├── skills/morning-operator/
│   ├── SKILL.md
│   └── references/
│       ├── execution-phases.md
│       └── report-format.md
├── agents/openai.yaml
└── README.md
```

## Run

After install, in any session say:

```
run morning operator
```

The skill auto-loads and the operator starts at Phase A.

## License

MIT.
