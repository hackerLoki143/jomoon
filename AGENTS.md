## Project rules

- All personal content (names, dates, letter text, WhatsApp number) lives in `src/lib/surprise.ts`; components read from it so edits happen in one place.
- Time-based states (birthday countdown, 11:11 unlock) are derived from a client-only clock in `Experience.tsx`; `?preview` shifts the clock to just before the unlock for rehearsal, so never gate logic on the real system time elsewhere.
- Animated visuals use CSS classes/keyframes defined in `src/styles.css` and canvas components; keep colors as tokens there.
