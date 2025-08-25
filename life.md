# Developer If–Then Playbook

Short, opinionated rules for this repo. Copy, paste, ship.

## Conventions
- If it starts with `use*`, it’s a React hook from this repo.
- If it’s in `utils/*`, it’s a pure function (no side effects).
- If you see `zod`, it’s a runtime schema validator.

---

## Dates & Time
- If you want to parse dates, please use `useDatey` (handles TZ + locale).
- If you want to format dates, please use `formatDate(date, "YYYY‑MM‑DD")`.
- If you want relative time (e.g., “3h ago”), please use `formatRelative(date)`.
- If you want a stable server timestamp, please use `Datey.nowUTC()`.
