# Molpha Documentation

Documentation for **Molpha** — verifiable data infrastructure that turns any HTTP API into a single threshold-signed payload, verified on Solana, EVM, and Starknet.

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
| **Documentation** | Start from developer journeys, then dive into agents, access models, gateways, verifiers, protocol specs, and migration notes |
| **SDK Reference** | `@molpha/sdk` overview, gateway API, and type reference |

### Documentation sidebar

```
Documentation/
├── Get Started/          # Home, introduction, how it works
├── Quickstarts/          # AI agents, smart contracts, backend, legacy producer flow
├── AI Agents/            # Agent overview and MCP integration
├── Access Models/        # Subscriptions, Delegates, x402 escrow
├── Core Concepts/        # Feeds, rounds & signatures, registry versions, payloads
├── Guides/               # Create/update, read/verify, EVM & Starknet verification
├── Gateways/             # Gateway overview and HTTP API
├── Verifiers/            # Solana, EVM, Starknet, deployments
├── Protocol/             # Architecture, cryptography, security
├── Operators/            # Run gateway infrastructure
├── Reference/            # Payload schema and specs
└── Resources/            # Glossary, FAQ, releases
```

## Contributing

1. Edit or add `.mdx` pages in the relevant folder.
2. Register new pages in the `navigation` section of `docs.json`.
3. Preview locally with `mintlify dev`.
4. Open a pull request.

## Resources

- [Mintlify Documentation](https://docs.mintlify.com)
- [@molpha/sdk on npm](https://www.npmjs.com/package/@molpha/sdk)
