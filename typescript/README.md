# @importantimport/material-color-utilities

[![npm package](https://img.shields.io/npm/v/@importantimport/material-color-utilities)](https://www.npmjs.com/package/@importantimport/material-color-utilities)

Algorithms and utilities that power the Material Design 3 (M3) color system,
including choosing theme colors from images and creating tones of colors; all in
a new color space.

See the upstream
[README](https://github.com/material-foundation/material-color-utilities#readme)
for more information.

## Getting started

```bash
pnpm add @importantimport/material-color-utilities # pnpm
yarn add @importantimport/material-color-utilities # yarn
npm i @importantimport/material-color-utilities # npm
```

```typescript
import { HCT } from '@importantimport/material-color-utilities'

// Simple demonstration of HCT.
const color = HCT.fromInt(0xff4285f4)
console.log(`Hue: ${color.hue}`)
console.log(`Chrome: ${color.chroma}`)
console.log(`Tone: ${color.tone}`)
```

### Theming

```typescript
import {
  argbFromHex,
  themeFromSourceColor,
  applyTheme,
} from '@importantimport/material-color-utilities'

// Get the theme from a hex color
const theme = themeFromSourceColor(argbFromHex('#f82506'), [
  {
    name: 'custom-1',
    value: argbFromHex('#ff0000'),
    blend: true,
  },
])

// Print out the theme as JSON
console.log(JSON.stringify(theme, null, 2))

// Check if the user has dark mode turned on
const systemDark = window.matchMedia('(prefers-color-scheme: dark)').matches

// Apply the theme to the body by updating custom properties for material tokens
applyTheme(theme, { target: document.body, dark: systemDark })
```

## Troubleshooting

If using node make sure to use the following flag:

```
node --experimental-specifier-resolution=node
```
