<h1 align="center">[Package Name]</h1>

<p align="center">
  <strong>[Brief tagline describing what the package does, ending with a demo/docs link. Try the <a href="https://bloxwap.github.io/[repo]/">live demo</a>.]</strong>
</p>

<p align="center">
  <a href="https://www.npmjs.com/package/@bloxwap/[package]"><img src="https://img.shields.io/npm/v/@bloxwap/[package]?style=flat-square" alt="npm version"></a>
  <a href="https://www.npmjs.com/package/@bloxwap/[package]"><img src="https://img.shields.io/npm/dm/@bloxwap/[package]?style=flat-square" alt="npm downloads"></a>
  <a href="https://codecov.io/gh/bloxwap/[repo]"><img src="https://img.shields.io/codecov/c/github/bloxwap/[repo]?style=flat-square" alt="Codecov"></a>
  <a href="https://bundlejs.com/?q=@bloxwap/[package]"><img src="https://img.shields.io/bundlejs/size/@bloxwap/[package]?style=flat-square" alt="bundle size"></a>
</p>

<!-- For non-JS-bundle packages (e.g. fonts), replace the last two badges with:
  <a href="https://github.com/bloxwap/[repo]/releases"><img src="https://img.shields.io/github/v/release/bloxwap/[repo]?style=flat-square" alt="release"></a>
  <a href="LICENSE"><img src="https://img.shields.io/github/license/bloxwap/[repo]?style=flat-square" alt="license"></a>
-->

## Features

- **[Feature headline].** [Full sentence explaining the feature and its benefit.]
- **[Another feature].** [Description with specifics, metrics, or comparisons where helpful.]
- **[More features].** [Use commas, periods, parentheses, or a spaced hyphen instead of em-dashes.]

## Installation

```sh
[npm install | bun install] @bloxwap/[package]
```

[ESM only | Works with] [Node.js [version] or newer | all modern browsers]. [Additional requirements or compatibility notes.]

## Release status

`[0.x.y]` is an early developer preview; expect breaking changes before `1.0`. [Add any specific caveats, limitations, or roadmap notes here.]

## Usage

[Brief introduction to the primary use case.]

```[language]
import { [exports] } from '@bloxwap/[package]';

// [Example usage with clear comments]
[code example]
```

[Additional usage patterns, edge cases, or common scenarios.]

```[language]
// [Another example showing different features]
[code]
```

## API

[Optional section. Include when the API is substantial or needs detail beyond inline usage examples.]

```ts
import {
  [function1], [function2], [function3],
  type [Type1], type [Type2],
} from '@bloxwap/[package]';
```

| Function | Description |
| --- | --- |
| `[function1]([params])` | [What it does, parameters, return value, and any important notes.] |
| `[function2]([params]?)` | [Description with optional params marked with `?`.] |

[Document types, options objects, constants, or exported utilities as needed.]

## Documentation

Guides, API reference, and examples: **https://bloxwap.github.io/[repo]/**

## Development

[Brief note about project structure if it's a workspace, or skip if a simple single package.]

```sh
[npm ci | bun install]
[npm | bun] test            # run the test suite
[npm | bun] run coverage    # tests with 100% line/branch/function coverage enforcement
[npm | bun] run dev         # dev server at http://localhost:[port]
```

[Note: The target is 100% line, branch, and function coverage. Use "tests with 100% line, branch, and function coverage enforcement" only when CI enforces it; otherwise state "coverage target is 100%".]

Requires [Node.js [version] or newer | Bun].

### Documentation dev-server ports

| Repository | Port |
| --- | --- |
| hyperliquid | 3901 |
| chart | 3902 |
| sfx | 3903 |
| font | 3904 |
| haptic | 3905 |
| [new repos] | [3906+] |

## Security

[Optional. Include for packages that handle private keys, wallets, or sensitive cryptographic operations.]

**[Package name] handles [private keys | wallet operations | sensitive data].** [Specific security considerations, audit status, best practices, or warnings.]

## License

[MIT](LICENSE)
