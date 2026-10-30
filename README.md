# Logn

*Logn* (Icelandic: dead calm, windless). A small installable PWA for shifting state with visuals, breath and attention.

## Modes

- **Downshift**: a breath pacer. The circle grows on the inhale and shrinks on the exhale, with vibration cues (so it works eyes-closed) and a soft filtered-noise "breath" sound. Patterns: 4/6 (about 6 breaths a minute), 4/8 long exhale, double sigh, box 4·4·4·4. Built for post-training cool-downs.
- **Cool-down**: box breathing (4·4·4·4, or an ease-in that runs 3s sides for the first minute) over a Drift scene (Silk by default). Vibration and sound carry the box so you can keep your eyes on the scene; the flow slows on the holds, with a faint ring and a quarter-arc per side of the box as a guide.
- **Drift**: slow colour fields and a very slow outward particle flow, with a faint 10-second halo to breathe along to. For winding down before bed.
- **Lock-in**: a fixation-then-tracking drill. Hold your eyes on the dot for the first 40%, then follow it. Tap when it turns amber. Reports cues caught and reaction time. For pre-heavy-single focus.

Optional before/after check-ins (1 calm, 5 wired) log whether a session actually moved you.

**Measures** (Downshift and Cool-down): pulse over 60 seconds (typed in, with an optional 60s count timer) and a control pause (breathe out normally, press and hold the circle, let go at the first urge; no timer shown, capped at 90s) before and after. The home screen's *Cool-down comparison* averages pulse drop and control-pause change per setup, so Cool-down · Silk can be compared against Downshift · Box over a few sessions.

**Watch heart rate**: same approach as Ironlog's cardio, over Web Bluetooth's standard Heart Rate Service (Chrome on Android). Works with chest straps and any watch that broadcasts heart rate (Garmin, Polar, Coros and others; Wear OS via a broadcast app on the watch; not Apple Watch or Fitbit). Once connected, the pulse measure fills in live from a 10-second average, the session shows live bpm, and each Downshift or Cool-down session logs a 5-second trace with its low point. The last device is remembered and reconnected quietly.

## Design rules

- No flicker or strobing. Every change is slow or a single soft colour shift.
- Dark and low-brightness throughout.
- Screen stays awake during a session (Wake Lock).
- All data stays in the browser (localStorage); "Export data" gives a JSON file.

## Later

If it earns its place, Downshift becomes Ironlog's rest-timer and cool-down screen, and Lock-in its pre-set screen.
