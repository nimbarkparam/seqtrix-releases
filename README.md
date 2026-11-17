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

**Direct installer** (same app, not code-signed yet, so Windows may show a SmartScreen
warning; with a built-in auto-updater):

**https://seqtrix.com/download**

That link always resolves to the newest installer published on this repo's releases.

**New in 0.18.0:** buy Pro Lifetime in the app for $149 once, Pro with no end date, and
switch to it from a Pro pass in Settings. Full notes: https://seqtrix.com/whats-new

---

## What a sequence is built from

The main steps:

| Action | What it does |
|---|---|
| **Open Application** | Launches any `.exe` or URL, or brings an app that is already open to the front |
| **Close Application** | Graceful close on a running process tree |
| **Wait** | Pause for N seconds or until a clock time, or wait until an app is running, a file or folder exists, or the PC is online |
| **Type Text** | Types a string into the focused window, by pasting or key by key |
| **Press Key** | Sends a key or modifier combo (Ctrl+S, Win+L, Alt+Tab) |
| **Run Command** | Runs a CMD or PowerShell command, in a folder you choose |
| **System Action** | Shutdown, restart, sleep, lock, log out |
| **Media Control** | Play/pause, next, previous, volume |
| **Copy a folder** | Backs up a folder and its subfolders to another folder, a network folder or a USB drive found by its name; never deletes or moves anything |
| **Show Message** | Shows a Windows notification, or a window on top with Continue and Stop the run |
| **Security Lock** | AES-256 encrypt, hide, password-lock, or securely delete a file or folder |

The OS Action step can also keep the PC awake, turn off the screen, clear the clipboard,
or hide or show the taskbar.

Focus Lock blocks distracting apps and websites for 15 minutes to 8 hours, with Soft,
Firm or Hard strength. Soft is free; Firm, Hard and website blocking are on Advanced and
Pro.

Describe (AI) builds a sequence from a plain-English description. It is optional, a
one-time download of about 2 GB, and runs on the CPU with no graphics card. Voice
control: push-to-talk on every plan, hands-free on Advanced and Pro.

**85 built-in templates** ship with the app, 15 of them on the free plan, so the first
useful automation is about ten seconds away rather than an afternoon of reading docs.
There is also a curated library of 50+ ready-made commands for the Run Command action.

**Triggers:** hotkey, schedule, an app launching, a hot corner, file watcher (create /
modify / delete), system events (login, idle, return-from-idle), the PC locking,
unlocking, waking, going on battery or being plugged in, a drive you pick being plugged
in, or the Mini Mode floating launcher - an always-on-top ring with 8 slots that sits
over any window. File-watch, system-event, PC and drive triggers need Advanced or Pro.
**Run later** runs a sequence once, in a set number of minutes or at a clock time.

**Honest limitation, stated up front:** sequences run **strictly linearly**. There is no
branching to other steps, no loops and no parallel paths: a sequence runs its steps in
order. If your workflow needs real control flow, AutoHotkey or PowerShell is the better
tool, and we would rather tell you that here than have you find out after installing.

---

## Local and offline

Sequences run on your machine. There is no cloud execution, crash reports and usage
statistics are off until you turn them on, and the app works with no internet connection. Optional account sign-in exists for licensing
and cross-device sync of your sequences. To check your plan, the app also sends a hashed
device ID, plus your sign-in if you are signed in, at launch and about every 30 minutes,
and the direct installer's built-in updater checks this repository for new versions.

---

## Requirements

- Windows 10 or Windows 11, 64-bit
- No macOS, no Linux, no mobile, no web version

---

## Pricing

**Starter** is free forever. **Advanced** is $4.99 for 30 days or $49 for a year (₹299 /
₹2,990) and covers up to 50 sequences. **Pro** is $9.99 for 30 days or $99 for a year
(₹599 / ₹5,990) with unlimited sequences. **Pro Lifetime** is $149 once (₹8,990): Pro on
all your devices with no end date. Lifetime means the life of the product, not your life.

Every fresh install gets a **15-day Advanced trial** - no credit card, no signup.

**Passes are paid once for the period you choose.** Nothing auto-renews and there is
nothing to cancel: when a pass ends, it keeps running for 3 days of grace, then returns
to Starter unless you buy again; nothing is deleted. A pass covers 30 or 365 days; Pro
Lifetime has no end date.

Full breakdown: [seqtrix.com/pricing](https://seqtrix.com/pricing)

---

## About this repository

This repo is the **public release mirror**. It exists so the auto-updater in every copy
installed from seqtrix.com can fetch its manifest, and so the installer has a stable
public download URL. The Microsoft Store version updates through the Store. The
application source is private.

Each tagged release publishes:

| Asset | Purpose |
|---|---|
| `Seqtrix_<version>_x64-setup.exe` | Windows installer |
| `Seqtrix_<version>_x64-setup.nsis.zip` | Updater payload consumed by the auto-updater |
| `Seqtrix_<version>_x64-setup.nsis.zip.sig` | Signature, verified by the running app |
| `latest.json` | Updater manifest pointing at this repo's release assets |

Releases are cut by CI on every version tag: a Windows runner builds the bundle, signs
it with the updater key (the installer itself is not code-signed), generates
`latest.json`, and publishes here. Nobody uploads release files by hand.

The [`legal/`](./legal/) folder holds copies of the EULA, privacy policy and terms. The
current versions, and the refund policy, are on seqtrix.com: https://seqtrix.com/eula,
https://seqtrix.com/privacy, https://seqtrix.com/terms and
https://seqtrix.com/refund-policy.

**Support and bug reports:** help@seqtrix.com

---

## Links

- Website: **https://seqtrix.com**
- Microsoft Store: **https://apps.microsoft.com/detail/9P5JT0BXFPS9**
- Compare with other tools: **https://seqtrix.com/vs/autohotkey** · [Task Scheduler](https://seqtrix.com/vs/task-scheduler) · [Power Automate](https://seqtrix.com/vs/power-automate)
- Use-case guides: **https://seqtrix.com/use-cases**
- Templates: **https://seqtrix.com/templates**

Built by the Seqtrix team. Independent, and not affiliated with Microsoft - that name
appears here only to describe the platform Seqtrix runs on.
