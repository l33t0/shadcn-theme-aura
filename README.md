# Aura Theme for shadcn/ui

[Aura](https://github.com/daltonmenezes/aura-theme) ported to [shadcn/ui](https://ui.shadcn.com) CSS variables (OKLCH). Colors, typography, motion, and effects.

## Variants

| Variant                    | Background               | Colors      |
| -------------------------- | ------------------------ | ----------- |
| `aura-dark`                | Dark (`#15141b`)         | Vivid       |
| `aura-dark-soft-text`      | Dark (`#15141b`)         | Desaturated |
| `aura-soft-dark`           | Lighter dark (`#21202e`) | Vivid       |
| `aura-soft-dark-soft-text` | Lighter dark (`#21202e`) | Desaturated |

## Install

```bash
npm install @l33t0/shadcn-aura-theme --registry=https://npm.pkg.github.com
```

Or add to `.npmrc`:

```
@l33t0:registry=https://npm.pkg.github.com
```

Then `npm install @l33t0/shadcn-aura-theme`.

## Usage

Import a variant in your `globals.css`, replacing your existing theme variables:

```css
@import "@l33t0/shadcn-aura-theme/themes/aura-dark.css";
```

Other variants: `aura-dark-soft-text.css`, `aura-soft-dark.css`, `aura-soft-dark-soft-text.css`.

The bare import (`@l33t0/shadcn-aura-theme`) defaults to `aura-dark`.

### Extras

Add optional layers for the full design system:

```css
@import "@l33t0/shadcn-aura-theme/extras/tokens.css";  /* spot accents, depth layers, gradients */
@import "@l33t0/shadcn-aura-theme/extras/fonts.css";    /* Outfit + JetBrains Mono, typography scale */
@import "@l33t0/shadcn-aura-theme/extras/motion.css";   /* spring easing, durations, keyframes */
@import "@l33t0/shadcn-aura-theme/extras/effects.css";  /* aura glow, cursor blink, status pulse */
```

Or import everything at once:

```css
@import "@l33t0/shadcn-aura-theme/full";
```

### Tokens

| Token | Value | Usage |
| --- | --- | --- |
| `--bg-primary` | `#15141b` | Page background |
| `--bg-elevated` | `#1c1b26` | Cards, panels |
| `--bg-surface` | `#222131` | Hover states, active surfaces |
| `--text-primary` | `#edecee` | Headings, body text |
| `--text-secondary` | `#a09fa6` | Supporting text |
| `--text-tertiary` | `#6d6d6d` | Labels, muted text |
| `--accent-green` | `#61ffca` | Success states |
| `--accent-orange` | `#ffca85` | Warnings, tags |
| `--accent-pink` | `#f694ff` | Decorative accents |
| `--accent-blue` | `#82e2ff` | Informational accents |
| `--accent-red` | `#ff6767` | Errors, destructive |
| `--aura-1` | `#a277ff` | Primary gradient stop |
| `--aura-2` | `#8455d4` | Mid gradient stop |
| `--aura-3` | `#c4a1ff` | Light gradient stop |

### Typography

Fonts: **Outfit** (body, display) and **JetBrains Mono** (labels, tags, code).

| Class | Font | Weight | Size | Usage |
| --- | --- | --- | --- | --- |
| body (default) | Outfit | 300 | 0.95rem | Body text |
| `.font-display` | Outfit | 600 | 2.2rem | Headings |
| `.font-mono` | JetBrains Mono | 500 | inherit | Code/system text |
| `.label` | JetBrains Mono | 500 | 0.7rem | Section labels (uppercase) |
| `.tag` | JetBrains Mono | 400 | 0.65rem | Tags |

### Motion

| Variable | Value | Usage |
| --- | --- | --- |
| `--ease-spring` | `cubic-bezier(0.16, 1, 0.3, 1)` | All interactive transitions |
| `--duration-hover` | `0.3s` | Hover states |
| `--duration-element` | `0.4s` | Element transitions |
| `--duration-page` | `0.7s` | Page-load fade-ins |

### Effects

CSS classes for ambient effects:

- `.aura-glow` — ambient purple haze via pseudo-elements with pulsing animation
- `.cursor-blink` — terminal cursor blink (1s step-end)
- `.status-dot` — pulsing opacity (3s ease-in-out)
- `.avatar-ring` — continuous rotation (8s linear)

## Color Palette

### Vivid

| Role   | Hex       |
| ------ | --------- |
| Purple | `#a277ff` |
| Green  | `#61ffca` |
| Orange | `#ffca85` |
| Pink   | `#f694ff` |
| Blue   | `#82e2ff` |
| Red    | `#ff6767` |

### Soft

| Role   | Hex       |
| ------ | --------- |
| Purple | `#8464c6` |
| Green  | `#54c59f` |
| Orange | `#c7a06f` |
| Pink   | `#c17ac8` |
| Blue   | `#6cb2c7` |
| Red    | `#c55858` |

## License

MIT.

Colors from [Aura Theme](https://github.com/daltonmenezes/aura-theme) by Dalton Menezes (MIT).
