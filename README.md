# skill-guard

> A safety gate for ClawHub skill updates — diffs files and scores risk before anything gets applied.

## The problem
When you update AI skills via ClawHub, you're essentially running someone else's code. 
skill-guard checks what changed and blocks the update if it looks risky.

## How it works
1. Reads your installed skills from `.clawhub/lock.json`
2. Fetches the latest version of each skill
3. Diffs the files and runs risk heuristics
4. Blocks the update if the risk score is too high

## Install
npm install
npm link

## Usage
Run `skill-guard` from your ClawHub project directory.

## Feedback welcome
This was an experiment in vibe coding — built with GPT by someone with no prior coding experience.
If you have thoughts on the concept, the code quality, or anything else, 
open an Issue or leave a comment. All feedback appreciated.
