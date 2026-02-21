# Aura Theme for shadcn/ui

[Aura](https://github.com/daltonmenezes/aura-theme) ported to [shadcn/ui](https://ui.shadcn.com) CSS variables (OKLCH). All four variants.

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
