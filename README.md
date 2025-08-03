### 🩺 InchCare: Cross-Chain Medical Incidents & Insurance Settlement

**InchCare** is a decentralized medical incident reporting and insurance settlement protocol built across **Starknet, Filecoin, Stellar (Soroban), ICP, and Ethereum**. It leverages **1inch Fusion SDK+** to coordinate **cross-chain swaps and payouts** using hashlocks, timelocks, and custom escrow contracts.

* 🪙 ERC-20 utility token deployed on Starknet, Filecoin, Optimism and Arbitrum for token-gated access to healthcare services
* 🌐 Medical incidents immutably logged on Stellar using Soroban smart contracts
* 🔁 Insurance claims settled via 1inch Fusion+ swaps across Ethereum, Starknet, and Filecoin
* 💾 Encrypted medical records stored on Filecoin/IPFS, referenced on-chain
* ⛓️ Rate-limiting protocol on Ethereum Sepolia for secure API-like throttling
* 🪙 Integrating Etherlink, an EVM-compatible L2, into our 1inch Fusion+ workflow to enable efficient cross-chain swaps using our PPT ERC-20 utility token, already deployed on Arbitrum, Optimism (testnet & mainnet), and now on Etherlink testnet.
* 🌍 Frontend deployed via Internet Computer (ICP) and integration with 1inch Fusion SDK+.

Designed at ETHGlobal Unite DeFi to demonstrate real-world impact through cross-chain DeFi infrastructure for healthcare.

1inch: We use 1inch Fusion SDK+ to enable automated, trustless settlement of insurance claims by executing cross-chain swaps between ETH and our ERC-20 utility tokens deployed on Starknet and Filecoin. The SDK powers our resolver logic, allowing the best bidder to fulfill payouts securely and efficiently. Our ERC-20 tokens provide token-gated access to healthcare services, while medical incidents are immutably logged on Stellar using Soroban smart contracts. Encrypted medical records are stored on Filecoin/IPFS, with their content identifiers referenced on-chain. We’ve also implemented a rate-limiting protocol on Ethereum Sepolia to prevent abuse and simulate regulated API flows.


Stellar: We use Stellar and Soroban smart contracts to immutably log medical incidents and trigger cross-chain settlement flows. Once an incident is verified, an off-chain relayer uses the 1inch Fusion+ SDK to initiate a swap between Stellar-based reports and the Medi ERC-20 token on Ethereum, using a hashlock/timelock-based escrow system. This allows us to bridge actions from Stellar into Ethereum’s DeFi layer for insurance payouts and token-gated services.

Etherlink: We’re integrating Etherlink, an EVM-compatible L2, into our 1inch Fusion+ workflow to enable efficient cross-chain swaps using our PPT ERC-20 utility token, already deployed on Arbitrum, Optimism (testnet & mainnet), and now on Etherlink testnet. We demonstrate its use in a token-gated medical billing dApp, where the PPT token can be used for in-app actions like save, print, and email of medical invoices. The dApp showcases how 1inch Fusion+ can enable low-cost settlement and access control across L2s.

Vercel deployment: https://invoice-ppt-arb-test.vercel.app/


