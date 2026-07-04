# RPME — Gamified Workout Tracker PWA

RPME is a gamified, offline-first fitness tracker built as an installable Progressive Web App — no framework, no build step, no backend. Body measurements drive a character profile and progress visuals; training feeds an XP and reward economy layered on top of a genuinely useful strength- and body-tracking core.

**Live demo:** https://finnraae.github.io/workout-pwa/

## Highlights

- **Single-file architecture** — the entire app is one `index.html` (~370 KB) of vanilla JavaScript and CSS custom properties. `Chart.js` (CDN) is the only runtime library. No bundler, no npm, no server.
- **Installable PWA** — service worker + web manifest make it installable to a phone home screen and fully usable offline; the service worker runtime-caches Chart.js and web fonts so charts and typography survive with no connection.
- **Local-first data** — all state persists in `localStorage`, with a JSON backup/restore flow to move data between devices.

## Body & measurement tracking

- Full **body-measurement tracking** — waist, chest, arms, and more, entered over time
- **Body-fat estimation** via the US Navy circumference method
- **Measurement history** rendered as radar and trend charts
- **Before/after progress photos**

## Training features

- **Progressive overload tracking** with automatic next-session weight/rep recommendations
- **1RM estimation** (Epley formula) and strength-level classification by bodyweight ratio
- **Exercise swap system** — alternatives and low-impact substitutions per movement
- **Supersets** with a shared rest timer, plus automatic deload detection
- **Soreness tracking** across muscle groups

## Gamification layer

- XP, coin economy, and a gacha-driven reward system (gear, pets, achievements)
- Achievement tiers and weekly boss-battle goals tied to real training consistency

## Polish

Haptic feedback (Vibration API), pull-to-refresh, an onboarding flow, dark mode, and a markdown export designed to be handed to an AI coach for feedback.

## Structure

| Path | App |
|------|-----|
| `/` | RPME — main fitness tracker |
| `/meal` | Companion meal / nutrition tracker |

## Tech

Vanilla JavaScript · HTML · CSS custom properties · Chart.js · Service Workers · Web App Manifest · localStorage

---

Built and maintained by [Finn Raae](https://github.com/finnraae).
