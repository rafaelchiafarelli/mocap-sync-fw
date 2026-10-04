# baseline — mocap-sync-fw

> **Parked.** Not scheduled — no LED hardware, and sync is done on the recorder's host clock. Kept as a future option; revisit only with a measured, clear improvement over timestamp sync.

**Goal:** ESP32 firmware that fires a short, intense LED flash on a serial command, visible on every camera.

**Scope:** PlatformIO + Arduino framework (proposal — to confirm), line-based serial protocol, LED pulse through a MOSFET.

**Out of scope:** Hardware trigger for cameras, networking, PoE.

**Initiative gate:** `PING`/`FLASH` respond over serial; the flash shows up in video from every camera at 3 m.

General context, cross-repository order and open questions:
`mocap-studio/HANDOFF.md`.
