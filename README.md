# Material Color Utilities

A fork of [`@material/material-color-utilities`](https://github.com/material-foundation/material-color-utilities/tree/main/typescript) to fix bugs and (maybe) add features.

This repository maintains only the TypeScript version: [`@importantimport/material-color-utilities`](https://github.com/importantimport/material-color-utilities/tree/dev/typescript)

Go to [Package README](/typescript/README.md) for more information.

## Bug fixes

- Use unbuild instead of tsc, fix [#35](https://github.com/material-foundation/material-color-utilities/issues/35) and provide CommonJS support [`f1b2651`](https://github.com/importantimport/material-color-utilities/commit/f1b2651ec6efb7778d6c358d93a126e33d211eeb)
  - https://github.com/material-foundation/material-color-utilities/issues/35
  - https://github.com/material-foundation/material-color-utilities/issues/68
  - https://github.com/material-foundation/material-color-utilities/issues/79
- Fix on-error-container in dark scheme [`1ff7904`](https://github.com/importantimport/material-color-utilities/commit/1ff79042462077f860a5cb30cdd58763723b4da6)
  - https://github.com/material-foundation/material-color-utilities/issues/62
- Fix Incorrect Array size in score.ts [`b4b67d4`](https://github.com/importantimport/material-color-utilities/commit/b4b67d4d09ffd688a09f3ac3f16642f6c2012776)
  - https://github.com/material-foundation/material-color-utilities/issues/46

## Chore

- Export all available utils [`d6ead76`](https://github.com/importantimport/material-color-utilities/commit/d6ead7686b264dfc4ab6216d7fbe2e76fdd011ea)
