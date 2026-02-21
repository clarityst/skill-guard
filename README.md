\# skill-guard



Safety gate for ClawHub skill updates (diff + risk heuristics).



\## What it does

\- Reads installed skills from `.clawhub/lock.json`

\- Pulls the latest version metadata via `clawhub inspect`

\- Installs the candidate version into a temp dir

\- Computes file diff vs your local installed version

\- Runs simple risk heuristics (exec/network hints, etc.)

\- Blocks update if risk score exceeds threshold



\## Install (local dev)

```bash

npm install

npm link

