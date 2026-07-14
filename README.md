# Molpha Documentation

Documentation for the **Molpha Oracle Protocol** — a pull-native threshold oracle that turns any HTTP API into a single threshold-signed result, verified on Solana, EVM, and Starknet.

Built with [Mintlify](https://mintlify.com).

## Local Development

Install the Mintlify CLI:

```bash
npm i -g mintlify
```

Run the docs locally from the repo root (where `docs.json` lives):

```bash
mintlify dev
```

The site will be available at `http://localhost:3000`.

## Site Structure

Navigation uses two top-level tabs:

| Tab | Purpose |
| --- | --- |
| **Documentation** | Learn the protocol, follow guides, set up the MCP server, read verifier and protocol specs |
| **SDK Reference** | `@molpha-oracle/sdk` overview, gateway API, and type reference |

### Documentation sidebar

```
Documentation/
├── Get Started/          # Home, introduction, quickstart, how it works
├── Core Concepts/        # Jobs, rounds & signatures, registry versions
├── Guides/               # Create/update, read/verify, EVM & Starknet verification
├── MCP Server/           # AI agent integration (Cursor, Claude, Codex)
├── Verifiers/            # Solana, EVM, Starknet, deployments
├── Protocol/             # Architecture, gateway, cryptography, security
└── Resources/            # Glossary, FAQ, releases
```

## Contributing

1. Edit or add `.mdx` pages in the relevant folder.
2. Register new pages in the `navigation` section of `docs.json`.
3. Preview locally with `mintlify dev`.
4. Open a pull request.

## Resources

- [Mintlify Documentation](https://docs.mintlify.com)
- [@molpha-oracle/sdk on npm](https://www.npmjs.com/package/@molpha-oracle/sdk)
