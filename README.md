# dexalot-public-chain-assets

This repo holds information about Dexalot L1 chains.

| Chain Name         | Chain Id |
|--------------------|----------|
| Dexalot L1 Testnet |  432201  |
| Dexalot L1 Mainnet |  432204  |

Each chain in the `chains` folder may contain the following files:
- `chain-information.json`: General information about the chain such as the
  name, vm configuration, and token configuration.
- `token-list.json`: A list of token contracts that exist on the chain with
  information about each. These tokens have been verified using the contract
  verifier at https://subnets.avax.network/tools/verify-contract.
- `gensesis.json`: For chains configured using
  [Subnet EVM](https://github.com/ava-labs/subnet-evm), this contains the
  genesis configuration parameters.
- `upgrade.json`: Contains network upgrades for the chain. For more
  information, see 
  https://docs.avax.network/subnets/subnet-upgrade#network-upgrades.
- `airdrop.json`: Contains a list of addresses that were airdropped tokens in genesis. Note: this file must be referenced in the chain config and the hash must be specified in genesis.
