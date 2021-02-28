# Earthswap Interface

[![Lint](https://github.com/Earthswap/earthswap-interface/workflows/Lint/badge.svg)](https://github.com/Earthswap/earthswap-interface/actions?query=workflow%3ALint)
[![Tests](https://github.com/Earthswap/earthswap-interface/workflows/Tests/badge.svg)](https://github.com/Earthswap/earthswap-interface/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)

An open source interface for Earthswap -- a protocol for decentralized exchange of Ethereum tokens.

- Website: [earthswap.net](https://earthswap.net/)
- Interface: [app.earthswap.net](https://app.earthswap.net)
- Docs: [earthswap.net/docs/](https://earthswap.net/docs/)
- Twitter: [@EarthswapProtocol](https://twitter.com/EarthswapProtocol)
- Reddit: [/r/Earthswap](https://www.reddit.com/r/Earthswap/)
- Email: [contact@earthswap.net](mailto:contact@earthswap.net)
- Discord: [Earthswap](https://discord.gg/FCfyBSbCU5)
- Whitepaper: [Link](https://hackmd.io/C-DvwDSfSxuh-Gd4WKE_ig)

### Accessing the Earthswap Interface

To access the Earthswap Interface, use an IPFS gateway link from the
[latest release](https://github.com/Earthswap/earthswap-interface/releases/latest), 
or visit [app.earthswap.net](https://app.earthswap.net).

## Listing a token

Please see the
[@earthswap/default-token-list](https://github.com/earthswap/default-token-list) 
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
[Earthswap V2](https://earthswap.net/docs/v2/smart-contracts/factory/) and 
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.** 
CI checks will run against all PRs.

## Accessing Earthswap Interface V1

The Earthswap Interface supports swapping against, and migrating or removing liquidity from Earthswap V1. However,
if you would like to use Earthswap V1, the Earthswap V1 interface for mainnet and testnets is accessible via IPFS gateways 
linked from the [v1.0.0 release](https://github.com/Earthswap/earthswap-interface/releases/tag/v1.0.0).
