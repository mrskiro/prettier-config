# @mrskiro/prettier-config

My personal Prettier configuration for consistent code formatting across all projects.

This package follows the [official Prettier documentation for sharing configurations](https://prettier.io/docs/sharing-configurations).

## Installation

Install the package as a development dependency:

```bash
# npm
npm install --save-dev @mrskiro/prettier-config

# yarn
yarn add --dev @mrskiro/prettier-config

# pnpm
pnpm add --save-dev @mrskiro/prettier-config
```

## Usage

Reference the configuration in your `package.json`:

```json
{
  "prettier": "@mrskiro/prettier-config"
}
```

Or in your `.prettierrc`:

```json
"@mrskiro/prettier-config"
```

### Extending the Configuration

If you need to override some options, you can extend the configuration in your `.prettierrc.mjs`:

```js
import prettierConfig from "@mrskiro/prettier-config";

/**
 * @type {import("prettier").Config}
 */
const config = {
  ...prettierConfig,
  semi: false, // Override specific options
};

export default config;
```

## License

MIT
