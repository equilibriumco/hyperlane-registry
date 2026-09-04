---
'@hyperlane-xyz/registry': minor
---

Added the Midnight stagenet chain entry and the NIGHT/midnight-sepolia warp
route, and recorded the entry's non-obvious fields inline: that Midnight has no
EVM chain id so `chainId` is a chosen value shared with devnet, that
`midnightNetworkId` is required by the SDK but absent from the schema, and that
the websocket node URL sits under `http` because the schema requires that field
while the agents ignore the value entirely — reads go through `gatewayUrls`.
