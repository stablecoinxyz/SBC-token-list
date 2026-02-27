# SBC Token List

The official token list for [Stable Coin (SBC)](https://stablecoin.xyz), maintained across multiple blockchain networks.

## Token List

`sbc-token-list.json` follows the standard token list format and can be consumed directly by wallets, DEXs, and other DeFi applications.

**Logo URI:** `ipfs://Qmei6RQgkLNjS2FsTgryBZ41Z9dqMrRV4WMtEgffgjwiRs`

## Deployments

| Network          | Chain ID | Address                                      | Decimals |
|------------------|----------|----------------------------------------------|----------|
| Ethereum         | 1        | `0xf9FB20B8E097904f0aB7d12e9DbeE88f2dcd0F16` | 18       |
| Optimism         | 10       | `0xf9FB20B8E097904f0aB7d12e9DbeE88f2dcd0F16` | 18       |
| Polygon          | 137      | `0xfdcC3dd6671eaB0709A4C0f3F53De9a333d80798` | 18       |
| Base             | 8453     | `0xfdcC3dd6671eaB0709A4C0f3F53De9a333d80798` | 18       |
| Arbitrum         | 42161    | `0xfdcC3dd6671eaB0709A4C0f3F53De9a333d80798` | 18       |
| Celo             | 42220    | `0xDE093684c796204224BC081f937aa059D903c52a`  | 18       |
| Avalanche        | 43114    | `0xf9FB20B8E097904f0aB7d12e9DbeE88f2dcd0F16` | 18       |
| Ethereum Classic | 61       | `0xfdcC3dd6671eaB0709A4C0f3F53De9a333d80798` | 18       |
| Solana           | 101      | `DBAzBUXaLj1qANCseUPZz4sp9F8d2sc78C4vKjhbTGMA` | 9     |
| Stellar          | —        | `SBC-GCQCNWT22JDLENQAVIE6DRJGHWAQ6EX2H5ABGPV55EJUPPZM5UA7KHZR` | 18 |

## Usage

Reference the raw token list URL directly in your application:

```
https://raw.githubusercontent.com/stablecoinxyz/SBC-token-list/main/sbc-token-list.json
```

## Contributing

To add a new network deployment or update token metadata, edit `sbc-token-list.json` and increment the `version` field:

- `patch` — metadata changes (logo, website, etc.)
- `minor` — new network added
- `major` — address change or network removed

Also update the `timestamp` to the current date.
