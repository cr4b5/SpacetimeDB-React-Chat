# kiloChat

A real-time chat application built with [SpacetimeDB](https://spacetimedb.com), React, and TypeScript.

Users can connect, set a display name, send messages, and see who is online — all powered by SpacetimeDB for persistent state and real-time sync.

## Prerequisites

- [Node.js](https://nodejs.org/) (v18+)
- [SpacetimeDB CLI](https://spacetimedb.com/install)

## Getting Started

1. Install dependencies:

```bash
npm install
```

2. Start a local SpacetimeDB instance and publish the server module:

```bash
npm run spacetime:publish:local
```

3. Start the development server:

```bash
npm run dev
```

## Project Structure

```
├── src/                    # React client application
│   ├── App.tsx             # Main chat UI component
│   ├── main.tsx            # Entry point with SpacetimeDB provider
│   ├── module_bindings/    # Auto-generated SpacetimeDB bindings
│   └── ...
├── spacetimedb/            # SpacetimeDB server module
│   └── src/index.ts        # Server-side schema, reducers, and lifecycle
├── package.json
└── ...
```

## Available Scripts

- `npm run dev` — Start the Vite dev server
- `npm run build` — Type-check and build for production
- `npm run preview` — Preview the production build
- `npm run test` — Run tests with Vitest
- `npm run lint` — Run ESLint and Prettier checks
- `npm run format` — Format code with Prettier
- `npm run spacetime:generate` — Regenerate TypeScript bindings from the server module
- `npm run spacetime:publish:local` — Publish the server module to a local SpacetimeDB instance
- `npm run spacetime:publish` — Publish the server module to SpacetimeDB maincloud

## License

Apache 2.0 — see [LICENSE](./LICENSE).
