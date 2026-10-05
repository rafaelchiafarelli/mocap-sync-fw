# mocap-sync-fw

ESP32 firmware for an **LED flash sync marker**: a visible flash that every
camera films, giving a shared visual reference to line the videos up.

## Where it sits in the architecture

**Nowhere, for now: this repository is parked.** The baseline syncs all
cameras on the recorder PC's clock instead. Every frame carries a host
timestamp, and START/END markers are recorded in software (`mocap-capture`),
so no sync hardware is needed.

The flash would come back only if timestamp-only sync proves too imprecise
**and** a flash gives a measured, clear improvement. If it ever does, it
would be triggered by the recorder over serial, and `mocap-extract`'s
alignment would refine offsets from the flash frames.

## Status

Parked, not scheduled. The planned work (PlatformIO skeleton, serial
protocol, LED pulse) stays in [`initiatives/baseline/`](initiatives/baseline/baseline.md)
so it can be picked up later. The reasoning is in
`mocap-capture/initiatives/future/README.md`.
