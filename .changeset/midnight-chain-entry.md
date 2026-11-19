---
'@hyperlane-xyz/registry': minor
---

Added the Midnight preview chain entry, `midnightpreview` with domain and chain
id 1200, and recorded its non-obvious fields inline: that Midnight has no EVM
chain id so `chainId` is a chosen value kept equal to the domain id, that
`midnightNetworkId` is required by the SDK but optional in the schema, and
which reads go to the node and which to the indexer in `gatewayUrls`.
