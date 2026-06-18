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

## Repository Structure

```
.
├── docs.json              # Mintlify configuration (navigation, theme, metadata)
├── index.mdx              # Home page
├── getting-started/       # Introduction, quickstart, how it works
├── concepts/              # Jobs, rounds & signatures, registry versions
├── guides/                # Create/update, read/verify, verify on EVM & Starknet
├── sdk/                   # @molpha-oracle/sdk overview, gateway API, reference
├── verifiers/             # On-chain verification (Solana, EVM, Starknet, deployments)
├── protocol/              # Architecture, gateway, cryptography, security model
├── resources/             # Glossary, FAQ, releases
└── logo/                  # Logo and favicon assets
```

## Contributing

1. Edit or add `.mdx` pages in the relevant folder.
2. Register new pages in the `navigation` section of `docs.json`.
3. Preview locally with `mintlify dev`.
4. Open a pull request.

## Resources

- [Mintlify Documentation](https://docs.mintlify.com)
- [@molpha-oracle/sdk on npm](https://www.npmjs.com/package/@molpha-oracle/sdk)
