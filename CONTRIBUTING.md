# Contributing to Kuma UI

Thanks for your interest in contributing to Kuma UI! We appreciate your help and your efforts to make this project better. Here are some guidelines to help you get started.

## Development Setup

Our project uses `pnpm` and `turborepo`. Here's how you can set it up:

1. Clone the repository.
2. In the root directory, run `pnpm install` to install dependencies.
3. To use everything correctly, run `pnpm build` to compile the necessary packages.
4. Make your changes. If you modify the source code, make sure to build the project to see your changes in action.
5. If you make any modifications, please test your changes. We prefer new features to come with tests.
6. If you update the README, please run `node scripts/sync-files.js` from the root directory to sync changes.

## Package Structure

Our project is organized into several packages within the `packages` directory:

- **@kuma-ui/babel-plugin** : Prepares for static analysis. It identifies modules imported from Kuma and rewrites the syntax to make it easier to analyze statically.
- **@kuma-ui/compiler**: Extracts Style Props and converts them to CSS.
- **@kuma-ui/core**: Provides component groups. Processes Style Props that could not be analyzed statically.
- **@kuma-ui/system**: Serves as the core of the Styled System. Converts Style Props into actual CSS syntax.
- **@kuma-ui/sheet**: Stores extracted Style Props and applies the Theme.
- **@kuma-ui/next-plugin, @kuma-ui/webpack, @kuma-ui/vite**: Plugins for each framework.

## Writing Articles or Tutorials

We welcome and encourage community members to write articles or tutorials about Kuma UI. If you are interested, we are more than happy to support you. Please contact us on [Twitter](https://twitter.com/kuma__ui) or Discord(https://discord.gg/QrsQ4EPp7G).
