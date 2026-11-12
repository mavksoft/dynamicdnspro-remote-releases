# Changelog — DDNSPro Remote

All notable releases published in this repository.

## v1.1.1 — 2026-11-12

- Fix: remote scroll on macOS trackpads — wheel deltas are now normalized to
  Windows `WHEEL_DELTA` (120) units with a fractional remainder, instead of
  sending raw point deltas that produced sub-notch scroll on the host.

**Assets:** `DDNSProRemote-macOS-1.1.1.dmg` · `DDNSProRemote-macOS-1.1.1.dmg.sha256` · `DDNSProRemote-macOS-1.1.1.zip` · `DDNSProRemote-macOS-1.1.1.zip.sha256` · `visor_macos.json` · `visor_macos_appcast.xml`

## v1.1.0 — 2026-11-12

- New signed auto-updater (Ed25519 manifest + in-app progress UI) replacing Sparkle.
- File manager usable while a desktop session is open (`_FILES` state fix + hardening).
- "Wait until it comes back" — sessions survive remote reboots and reattach
  automatically, with a configurable timeout in Settings.
- Resolution selector in the session bar (admin-permitted profiles).
- RDP session picker auto-opens on multi-session hosts.
- Authenticated machine thumbnails + post-session `screen_thumb`.
- Logout confirmation dialog; clicking the username no longer logs out.
- Dock ghost icon and agent-icon cursor fixes.

**Assets:** `DDNSProRemote-macOS-1.1.0.dmg` · `DDNSProRemote-macOS-1.1.0.dmg.sha256` · `DDNSProRemote-macOS-1.1.0.zip` · `DDNSProRemote-macOS-1.1.0.zip.sha256` · `visor_macos.json` · `visor_macos_appcast.xml`

## v1.0.7 — 2026-11-12

- Stability and input-handling fixes.

## v1.0.6 — 2026-11-12

- Interim build: session reliability improvements.

## v1.0.4 / v1.0.5 — 2026-11-11

- First public builds of the native macOS viewer (Sparkle updates).
