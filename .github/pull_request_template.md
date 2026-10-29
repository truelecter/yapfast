## What and why

<!-- What changes for someone using Yapfast, and why. Link the issue it closes, if any. -->

## How it works

<!-- The approach, layer by layer where it crosses them (core, UI, worker, Discord, Matrix). Call out anything a reviewer could miss: new threads, locks, processes, protocol payloads. -->

## Memory

<!-- What the change holds or copies on a path that runs per event or per frame, and what was done to keep it lean. A change that saves memory gives the numbers it measured (docs/measurements/README.md). Write "No new per-frame or per-event work" when that's all there is. -->

## Checks

- [ ] `scripts/check --fast` passes
- [ ] `scripts/test-fake-discord` passes (for changes to `crates/yapfast-discord`, `discord_text` or `testing/fake_discord.ts`)
- [ ] Docs describe the new behaviour, in the same commit as the change
- [ ] Discord payloads match https://docs.discord.food, and the fake has the same shape

## Tested on

<!-- What you ran and saw: a ui-session, a real call, a real device. Say what wasn't tried. -->

- [ ] Linux
- [ ] Windows
- Not tried:
