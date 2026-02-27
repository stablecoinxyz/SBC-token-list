# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a data-only repository containing a token list for the SBC (Stable Coin) token across multiple blockchain networks. The sole file is `sbc-token-list.json`, which follows the standard token list format (similar to Uniswap token lists).

There are no build tools, test frameworks, or CI/CD pipelines.

## Token List Structure

`sbc-token-list.json` contains:
- **Top-level metadata**: `name`, `timestamp`, `version` (semver with `major`/`minor`/`patch` fields)
- **`tokens` array**: One entry per network deployment

Each token entry includes: `chainId` (integer), `address`, `name`, `symbol`, `decimals`, `logoURI` (IPFS), `extensions.website`, and `tags`.

**Exception**: The Stellar network entry uses `description: "Stellar-Pubnet"` instead of `chainId`, as Stellar doesn't use numeric chain IDs.

## Deployed Networks

| Network           | ChainId | Decimals |
|-------------------|---------|----------|
| Ethereum          | 1       | 18       |
| Optimism          | 10      | 18       |
| Polygon           | 137     | 18       |
| Arbitrum          | 42161   | 18       |
| Celo              | 42220   | 18       |
| Avalanche         | 43114   | 18       |
| Base              | 8453    | 18       |
| Ethereum Classic  | 61      | 18       |
| Solana            | 101     | 9        |
| Stellar           | (none)  | 18       |

## Versioning Convention

When modifying the token list, increment `version` according to semver semantics:
- **patch**: Metadata-only changes (e.g., logo, website)
- **minor**: New token added
- **major**: Token removed or address changed

Also update the `timestamp` to the current date in ISO 8601 format (`YYYY-MM-DDT00:00:00.000Z`).
