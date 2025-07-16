# LumorUI
A framework-agnostic clarity & accessibility layer for interoperable UI components.

lumor-ui is a React-first component library designed for signal-based, calm interfaces that prioritize accessibility, behavioral clarity, and interoperability over aesthetics.

# Why “Lumor”?

Inspired by lumen (light and yes, a cheeky nod to my own name :D ) and resonance (signal propagation), lumor-ui is a signal-driven interface layer for calm, intelligent frontends.


# Stack

React + TypeScript

Vite for fast bundling

ESLint with strict type-checked rules

Jest + Testing Library

TailwindCSS

# ESLint Setup

This repo uses the latest type-aware rules from @typescript-eslint for better dev ergonomics in production apps.

// eslint.config.js
export default tseslint.config([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Use strict + stylistic rules for production-grade quality
      ...tseslint.configs.strictTypeChecked,
      ...tseslint.configs.stylisticTypeChecked,
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
    },
  },
])

# Coming Soon

Component playground (Storybook)

Unit tests for every component

ARIA test suite

CI workflows (typecheck, lint, test)

# Vision

lumor-ui is not a full design system. It’s an interface bridge that helps engineers:

Ensure every UI behavior has a signal (keyboard, focus, screen reader)

Build components that integrate into any system (internal or open-source)

Reduce friction in accessible design implementation

# Author

Built with intent by Roshni (https://www.linkedin.com/in/rosh8/)