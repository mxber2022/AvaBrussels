# Teleporte Avalanche Chat App

A decentralized chat application to send, receive, and verify the receipt of messages using Teleporte Avalanche.

## Prefunding Details
- **Address:** `0x032C94D31aA165615D67E9b50aBDC023C37a54a1`
- **Balance:** `1,000,000,000,000,000,000,000,000`
- **ChainId:** `9876`
- **Token Symbol:** `hh`

## Browser Extension Connection Details
- **RPC URL:** `http://127.0.0.1:9650/ext/bc/2hmc4x65LAAggW72MuP5P3uMvSDZpY8yeVJjDsDLp7yntUGt35/rpc`
- **Funded Address 1:** `0x032C94D31aA165615D67E9b50aBDC023C37a54a1` with `1,000,000 (10^18)` 
  - **Private Key:** `24ce3b922964562754785bd24410a8a9c4f3bf8f88b4439ee671df1fece43a41`
- **Funded Address 2:** `0xb29EB2586EEAA910447B585F7F80A750d6d59731` with `600 (10^18)`
- **Network Name:** `hackerhouse`
- **Chain ID:** `9876`
- **Currency Symbol:** `hh`

## Local Network Blockchain ID
- `0xe044673607e04459fa548a747bb584de0f624837a2e6b38f4003537157a134b4`


### Key Interfaces

- **ITeleporterMessenger Interface**
  - `sendCrossChainMessage`: Called by contracts on the origin chain to initiate the sending of a message to a contract on another EVM instance.
  - `receiveCrossChainMessage`: Called by cross-chain relayers on the destination chain to deliver signed messages to the destination EVM instance.

- **ITeleporterReceiver Interface**
  - `receiveTeleporterMessage`: Called by the Teleporter contract on the destination chain to deliver a message to the destination contract.

  > **Note:** If a contract does not implement `ITeleporterReceiver`, but instead implements fallback, the fallback function will be called when Teleporter attempts to perform message execution. The message execution is marked as failed if the fallback function reverts, otherwise, it is marked as successfully executed.

## Features

- **Send Messages:** Users can send messages securely over the Avalanche network.
- **Receive Messages:** Users can receive messages in real-time.
- **Verify Messages:** Ensure message integrity and authenticity using blockchain technology.

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- Avalanche node (local or remote)


## Contributing

We welcome contributions! Please read our [contributing guidelines](CONTRIBUTING.md) for more details.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or support, please contact [yourname@example.com](mailto:yourname@example.com).

---

**Note:** This is a sample README template. Replace placeholders with actual information about your project.
