# On-Chain Governance DAO

This repository contains a robust, transparent governance framework inspired by Compound and OpenZeppelin's Governor standards. It enables a decentralized community to manage a treasury or modify protocol parameters without a central authority.

## Features
* **Proposal Lifecycle**: Handles the full flow from proposal creation to voting, success, and execution.
* **Voting Power**: Leverages ERC-20 snapshots or checkpoints to prevent "flash loan" attacks during votes.
* **Quorum & Thresholds**: Configurable settings for the minimum number of votes required for a proposal to pass.
* **Timelock Integration**: Includes a mandatory delay between a successful vote and execution to protect the community.

## Components
1. **GovernanceToken**: An ERC-20 token with `ERC20Votes` extension to track historical voting power.
2. **GovernorContract**: The logic engine that processes proposals and tallies votes.
3. **TimelockController**: A security layer that delays actions, giving users time to exit if they disagree with a passed proposal.

## License
MIT
