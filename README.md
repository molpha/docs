# Molpha Documentation

Documentation for **Molpha** — verifiable data infrastructure that turns any HTTP API into a single threshold-signed payload, verified on Solana, EVM, and Starknet.

Built with [Mintlify](https://mintlify.com).

## Contributor guide

The contributor guide is kept outside this repository, in `development-docs/` at the root of the multi-repository workspace: `protocol-structure.mdx`, `components.mdx` and `local-testing.mdx`. For coding agents in that workspace, start with the workspace-root `AGENTS.md`.

## Local development

Run the docs from the repo root (where `docs.json` lives) with the current Mintlify CLI:

```bash
npx mint@latest dev
```

The site is served at `http://localhost:3000`. An old globally installed `mintlify` or `mint` CLI can reject options in `docs.json` that the current schema allows; use the command above or update the CLI.

Check links before opening a pull request:

```bash
npx mint@latest broken-links
```

## Site structure

Navigation is defined in `docs.json` and has three tabs:

| Tab | Contents |
| --- | --- |
| **Documentation** | Quickstarts, concepts, access and payments, MCP server, verifiers, protocol, resources |
| **API reference** | Gateway API overview and one page per operation, generated from `gateway-openapi.yaml` |
| **SDK** | `@molpha/sdk` overview, gateway client and reference |

```
index.mdx          Home
quickstarts/       AI agents, backends, smart contracts
concepts/          Sources and feeds, attestations, registry versions
access-models/     Subscriptions, delegates, x402
mcp/               MCP server: overview, hosted, local, tools
verifiers/         Solana, EVM, Starknet, deployments
guides/            Maintain a feed
protocol/          Architecture, cryptography, Solana program, security model
resources/         Glossary, FAQ, releases
gateways/          Gateway API overview and operation stubs
sdk/               TypeScript SDK
```

## Contributing

1. Edit or add `.mdx` pages in the relevant folder.
2. Register new pages in the `navigation` section of `docs.json`.
3. Preview locally with `npx mint@latest dev`.
4. Open a pull request.

## Resources

- [Mintlify Documentation](https://docs.mintlify.com)
- [@molpha/sdk on npm](https://www.npmjs.com/package/@molpha/sdk)
