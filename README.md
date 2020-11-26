# Zingswap Interface

[![Tests](https://github.com/Uniswap/uniswap-interface/workflows/Tests/badge.svg)](https://github.com/Uniswap/uniswap-interface/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)

An open source interface for Zingswap -- a decentralized exchange on the Thundercore blockchain.

- Website: [zing.finance](https://about.zing.finance/)
- Interface: [swap.zing.finance](https://swap.zing.finance)
- Docs: [docs.zing.finance/docs/](https://swap.zing.finance/docs/zingswap)
- Telegram: [Zing Finance](https://t.me/zingfinance)

## Accessing the Zingswap Interface

To access the Zingswap Interface, use an IPFS gateway link from the
[latest release](https://github.com/zing-finance/zingswap-interface/releases/latest),
or visit [swap.zing.finance](https://swap.zing.finance).

## Listing a token

Please see the
[@zing-finance/default-token-list](https://github.com/zing-finance/default-token-list)
repository.

## Development

### Install Dependencies

```bash
yarn
```

### Run

```bash
yarn start
```

### Configuring the environment (optional)

To have the interface default to a different network when a wallet is not connected:

1. Make a copy of `.env` named `.env.local`
2. Change `REACT_APP_NETWORK_ID` to `"{YOUR_NETWORK_ID}"`
3. Change `REACT_APP_NETWORK_URL` to e.g. `"https://{YOUR_NETWORK_ID}.infura.io/v3/{YOUR_INFURA_KEY}"`

Note that the interface only works on testnets where both
[Uniswap V2](https://uniswap.org/docs/v2/smart-contracts/factory/) and
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.**
CI checks will run against all PRs.

## Accessing TTSwap interface

The Zingswap Interface supports swapping against, and migrating or removing liquidity from TTSwap.
