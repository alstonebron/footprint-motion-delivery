# Footprint Motion Template — v4

Flagship motion template. SolarEdge-scale structure with Footprint content and an award-tier (Awwwards-style) motion system. Single file + assets, zero dependencies.

**Live:** https://dsh.growwithfootprint.com/cinematic/templates/footprint-motion/index.html

## Structure
Hero video → Core pillars → Stats band (+ kinetic text) → Six leaks → Leak picker → Work tabs → Image carousel strip → Services → Grove cards → Free scan → Final CTA → Footer (+ marquee)

## Effect vocabulary (reusable classes)

| Class / feature | Effect |
|---|---|
| `.rv` | Fade-up on scroll |
| `.fly-l / .fly-r / .fly-u / .fly-d` | Directional fly-in, 170px travel ±8° rotation |
| `.spin-l / .spin-r` | 3D Y-axis spin-in, 115° + 150px travel |
| `.flip-in` | X-axis flip-up, 105° with overshoot spring |
| `.fold-in` | Fold down from top edge (paper fold) |
| `.clip-reveal .clip-lr/.clip-rl/.clip-tb` | Clip-path image wipe (directional) |
| `.rowfade` | Simple row fade |
| `.kb` | Ken Burns infinite zoom/pan on img |
| `.tiltable` | Mouse 3D tilt, 17° max + lift/scale |
| `.mag` | Magnetic mouse pull (42%) + cursor morph |
| `.sheen` / pillar/leak/gcard ::after | Light streak sweep on hover |
| `.marquee` | Infinite ticker (pauses on hover) |
| `.kinetic` | Giant outlined text scrolling behind section |
| `.strip` | Skewed auto-scroll image carousel (pauses on hover) |
| `[data-scramble]` | Text scramble/decode on load |
| `#heroHeadline` | Split-word reveal (JS) + scroll count-up `.cnt` |
| `.loader` | Intro curtain with progress bar |
| scroll velocity | Cards skew up to 5° with scroll speed |

## Customization
- Colors: `:root` CSS variables (`--amber` is the accent).
- Copy/leaks: `LEAKS` array in the script block.
- Carousel: `.strip-track` cells — duplicate any block of cells; animation translates -50%.
- All motion respects `prefers-reduced-motion`; pointer effects disabled on touch.

## Versions
- v1 — structure, hero video, mega menu, leak picker
- v2 — cursor, magnetic, tilt, marquee, sheen, split text, scramble, parallax, skew
- v3 — directional fly-ins, 3D spin-ins, flips, clip reveals, loader curtain
- v4 — exaggerated amplitudes, Ken Burns, carousel strip, fold-in rows, kinetic text
