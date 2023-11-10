# Fetch the NFT bot

This repository implements a Discord bot with the `fetch-nft` library from Audius. It will allow you to pass in an ETH or SOL wallet and be returned the user's collectibles.

## Usage
`/fetch` launch the fetch NFT tool
  - Then select ETH or SOL network and input appropriate wallet address
  - The UI will not allow you to input the incorrect wallet length

The bot will return any number of collectibles for a given wallet on Ethereum or Solana networks.

## Workarounds

The `getEthereumCollectibles` and similar functions rely on a deprecated version of the openSeaAPI and this has broken their functionality. [Source](https://docs.opensea.io/v1.0/changelog/api-v2-fully-supported)

I've implemented the latest version of the `openSeaAPI` with `fetch` to achieve this functionality. The relevant `fetch-nft` code is commented out in `index.js` lines 79-84
