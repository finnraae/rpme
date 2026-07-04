# Workout Tracker PWA

A gamified, offline-first workout tracker built as an installable Progressive Web App — no framework, no build step, no backend. Body measurements drive a character profile; training feeds an XP and reward economy on top of a genuinely useful strength-tracking core.

**Live demo:** https://finnraae.github.io/workout-pwa/

## Highlights

- **Single-file architecture** — the entire app is one `index.html` of vanilla JavaScript and CSS custom properties, with `Chart.js` (CDN) the only dependency. No bundler, no npm, no server.
- **Installable PWA** — service worker + web manifest make it installable to a phone home screen and fully usable offline.
- **Local-first data** — all state persists in `localStorage`; a JSON backup/restore flow lets the user move data between devices.

## Training features

- **Progressive overload tracking** with automatic next-session weight/rep recommendations
- **1RM estimation** via the Epley formula, with strength-level classification by bodyweight ratio
- **Exercise swap system** — alternatives and low-impact substitutions per movement
- **Supersets** with a shared rest timer, plus automatic deload detection
- **Soreness tracking** and body-fat estimation (US Navy circumference method)
- **Measurement history** rendered as radar and trend charts; before/after progress photos

## Gamification layer

- XP, coin economy, and a gacha-driven reward system (gear, pets, achievements)
- Achievement tiers and weekly boss-battle goals tied to real training consistency

## Polish

Haptic feedback (Vibration API), pull-to-refresh, an onboarding flow, dark mode, and a markdown export designed to be handed to an AI coach for feedback.

## Structure

| Path | App |
|------|-----|
| `/` | Workout tracker (main app) |
| `/meal` | Companion meal / nutrition tracker |
| `/rpg` | RPG-mode variant |

## Tech

Vanilla JavaScript · HTML · CSS custom properties · Chart.js · Service Workers · Web App Manifest · localStorage

---

Built and maintained by [Finn Raae](https://github.com/finnraae).
