# skill-guard

Safety gate for ClawHub skill updates (diff + risk heuristics).

## What it does
- Reads installed skills from `.clawhub/lock.json`
- For each skill: fetches latest version, diffs files, runs simple risk heuristics
- Blocks update if risk score is above threshold

⚠️ Run `skill-guard` from (or point `--workdir` to) a ClawHub-managed project directory that contains `.clawhub/lock.json` (e.g. your OpenClaw project), not from the `skill-guard` repo itself.

## Install (dev)
```bash
npm install
npm link
