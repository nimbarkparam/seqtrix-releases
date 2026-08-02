# Seqtrix

**No-code Windows automation, with file security built into the workflow.**

[![Get Seqtrix from the Microsoft Store](https://img.shields.io/badge/Microsoft%20Store-Download-0078D4?logo=microsoft&logoColor=white)](https://apps.microsoft.com/detail/9P5JT0BXFPS9)
[![Website](https://img.shields.io/badge/seqtrix.com-Website-6366f1)](https://seqtrix.com)
[![Latest release](https://img.shields.io/github/v/release/nimbarkparam/seqtrix-releases?label=latest)](https://github.com/nimbarkparam/seqtrix-releases/releases/latest)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-lightgrey)](https://seqtrix.com/download)

Seqtrix turns the repetitive things you do on Windows into named, reusable
**sequences**. Drag actions onto a canvas - open an app, wait, type text, press a key,
run a command, control media, lock a file - chain them in order, and fire the whole
thing from a hotkey, a schedule, a file change, an app launching, or a floating
launcher ring that sits on top of every window.

It is the middle ground between doing it by hand and learning to write scripts: more
capable than Task Scheduler, which can only launch one program, and simpler than
AutoHotkey, which is a programming language.

**The part nothing else in the category has:** a Security Lock action that
AES-256-encrypts, hides, password-locks, or securely deletes a file or folder *as a step
inside the automation*. Windows 11 still cannot password-protect a folder. Seqtrix can,
and it can do it on a schedule.

---

## Install

**Recommended - Microsoft Store** (one click, no SmartScreen warning, Store-managed
updates):

**https://apps.microsoft.com/detail/9P5JT0BXFPS9**

**Direct installer** (same app, code-signed, with a built-in auto-updater):

**https://seqtrix.com/download**

That link always resolves to the newest installer published on this repo's releases.

---

## What a sequence is built from

There are **9 action types**:

| Action | What it does |
|---|---|
| **Open Application** | Launches any `.exe` or URL |
| **Close Application** | Graceful close on a running process tree |
| **Wait** | Pause for N seconds, or until a wall-clock time |
| **Type Text** | Types a string into the focused window |
| **Press Key** | Sends a key or modifier combo (Ctrl+S, Win+L, Alt+Tab) |
| **Run Command** | Runs a CMD or PowerShell command |
| **System Action** | Shutdown, restart, sleep, lock, log out |
| **Media Control** | Play/pause, next, previous, volume |
| **Security Lock** | AES-256 encrypt, hide, password-lock, or securely delete a file or folder |

**80 built-in templates** ship with the app, so the first useful automation is about ten
seconds away rather than an afternoon of reading docs. There is also a curated library of
50+ ready-made commands for the Run Command action.

**Triggers:** hotkey, schedule, file watcher (create / modify / delete), system events
(login, idle, return-from-idle), or the Mini Mode floating launcher - an always-on-top
ring with 8 slots that sits over any window.

**Honest limitation, stated up front:** sequences run **strictly linearly**. There is no
branching, no loops, no conditionals, no retries, and no parallel paths. If your workflow
needs real control flow, AutoHotkey or PowerShell is the better tool, and we would rather
tell you that here than have you find out after installing.

---

## Local and offline

Sequences run on your machine. There is no cloud execution, no telemetry by default, and
the app works with no internet connection. Optional account sign-in exists for licensing
and cross-device sync of your sequences; that is the only thing that talks to a server.

---

## Requirements

- Windows 10 or Windows 11, 64-bit
- No macOS, no Linux, no mobile, no web version

---

## Pricing

**Starter** is free forever. **Advanced** is $7.99/month or $79/year (₹299 / ₹2,990) and
covers up to 50 sequences. **Pro** is $14.99/month or $149/year (₹599 / ₹5,990) with
unlimited sequences.

Every fresh install gets a **15-day Advanced trial** - no credit card, no signup.

**One-time payment for the period you choose.** Nothing auto-renews and there is nothing
to cancel: when the period ends, access simply reverts to Starter unless you buy again.
One payment covers 30 or 365 days - it is not a lifetime licence.

Full breakdown: [seqtrix.com/pricing](https://seqtrix.com/pricing)

---

## About this repository

This repo is the **public release mirror**. It exists so the auto-updater in every
installed copy of Seqtrix can fetch its manifest anonymously, and so the installer has a
stable public download URL. The application source is private.

Each tagged release publishes:

| Asset | Purpose |
|---|---|
| `Seqtrix_<version>_x64-setup.exe` | Windows installer |
| `Seqtrix_<version>_x64-setup.nsis.zip` | Updater payload consumed by the auto-updater |
| `Seqtrix_<version>_x64-setup.nsis.zip.sig` | Signature, verified by the running app |
| `latest.json` | Updater manifest pointing at this repo's release assets |

Releases are cut by CI on every version tag: a Windows runner builds and signs the
bundle, generates `latest.json`, and publishes here. Nobody commits to this repo by hand.

The [`legal/`](./legal/) folder mirrors the EULA, privacy policy, terms, and refund
policy that the app and website link to.

**Support and bug reports:** support@seqtrix.com

---

## Links

- Website: **https://seqtrix.com**
- Microsoft Store: **https://apps.microsoft.com/detail/9P5JT0BXFPS9**
- Compare with other tools: **https://seqtrix.com/vs/autohotkey** · [Task Scheduler](https://seqtrix.com/vs/task-scheduler) · [Power Automate](https://seqtrix.com/vs/power-automate)
- Use-case guides: **https://seqtrix.com/use-cases**
- Templates: **https://seqtrix.com/templates**

Built by [Param Nimbark](https://seqtrix.com/about). Independent, and not affiliated with
Microsoft - that name appears here only to describe the platform Seqtrix runs on.
