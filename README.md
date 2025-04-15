![Cover](.github/cover.png)

# Core Contracts - Bug Bounty

This repository is a slimmed-down version of Haven1's Core Smart Contract codebase.
It contains only the essential smart contracts and interfaces required for security
auditing as part of our public bug bounty program.

By excluding auxiliary infrastructure, off-chain tooling, and non-critical
modules, we aim to provide security researchers with a clean and minimal
environment that emphasizes the core protocol logic. This approach reduces noise,
improves readability, and allows for more effective and efficient review of the
contracts most critical to the protocol’s security and stability.

## Smart Contracts

All smart contracts can be found under the `contracts/` directory. Each contract
is thoroughly documented with in-line comments and NatSpec annotations to support
clear understanding and effective auditing. The structure is modular, and
interfaces are included where relevant to aid in reasoning about contract
interactions and system behavior.

```ml
.
├── airdrop
│   ├── AirdropClaim.sol
│   ├── interfaces
│   └── lib
├── bridge
│   ├── BridgeController.sol
│   ├── BridgeRelayer.sol
│   ├── LockedH1.sol
│   └── interfaces
├── external-chains
│   └── eth-mainnet
├── fee
│   ├── FeeContract.sol
│   ├── channels
│   ├── interfaces
│   └── lib
├── governance
│   ├── FeeDistributor.sol
│   ├── VotingEscrow.sol
│   └── interfaces
├── h1-developed-application
│   ├── H1DevelopedApplication.sol
│   ├── interfaces
│   └── lib
├── h1-native-application
│   ├── H1NativeApplication.sol
│   ├── H1NativeApplicationUpgradeable.sol
│   ├── H1NativeBase.sol
│   └── interfaces
├── network-guardian
│   ├── NetworkGuardian.sol
│   ├── NetworkGuardianController.sol
│   ├── interfaces
│   └── lib
├── nfts
│   └── Haven1LaunchCrew.sol
├── proof-of-identity
│   ├── ProofOfIdentity.sol
│   ├── interfaces
│   └── lib
├── staking
│   ├── SimpleStaking.sol
│   ├── Staking.sol
│   ├── interfaces
│   └── lib
├── test
│   └── FixedFeeOracle.sol
├── tokens
│   ├── BackedHRC20.sol
│   ├── EscrowedH1.sol
│   ├── HRC20.sol
│   ├── WH1.sol
│   └── interfaces
├── utils
│   ├── Address.sol
│   ├── OnChainRouting.sol
│   ├── Semver.sol
│   ├── interfaces
│   └── upgradeable
└── vendor
    └── uniswapV3
```
