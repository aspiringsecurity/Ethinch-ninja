### 🩺 InchCare: Cross-Chain Medical Incidents & Insurance Settlement

**InchCare** is a decentralized medical incident reporting and insurance settlement protocol built across **Starknet, Filecoin, Stellar (Soroban), Etherlink, ICP and Ethereum**. It leverages **1inch Fusion SDK+** to coordinate **cross-chain swaps and payouts** using hashlocks, timelocks, and custom escrow contracts.

* 🪙 PPT (Patient Pro Token) Utility token deployed on Starknet, Filecoin, Optimism and Arbitrum for token-gated access to healthcare services
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


Vercel Deployment

dapp for Patient Pro token deployment for token gated access on Optimism Mainnet + + 1inch fusion sdk+ swap usage: https://invoice-ppt-op-mainnet.vercel.app/

dapp for Patient Pro Token deployment for token gated access on Starknet blockchain + 1inch fusion sdk+ swap usage: https://cairo-invoice-frontend.vercel.app/

dapp for Patient Pro token deployment for token gated access on Filecoin blockchain + + 1inch fusion sdk+ swap usage: https://web3-invoice-token-gated-storacha.vercel.app and 
https://fil-token-gated-dapp-storacha.vercel.app (Filecoin Mainnet)

dapp for Patient Pro token deployment for for token gated access on Arbitrum testnet + + 1inch fusion sdk+ swap usage: https://invoice-ppt-arb-test.vercel.app/




Steps to Swap between EVM (Eth) and Non-EVM (FIL, STRK) Chains using 1inch fusion+ sdk

Please visit: https://github.com/aspiringsecurity/Inch-Care/tree/main/1inch-fusion-sdk%2B-ETH-FIL-STRK-extn/1inch-fusion-sdk%2B-FIL-extension


Contract Addresses + + 1inch fusion sdk+ swap usage

Please visit: 

1. https://github.com/aspiringsecurity/Inch-Care/tree/main/1inch-fusion-sdk%2B-ETH-FIL-STRK-extn (Filecoin and Starknet Blockchain)

Demo and Screencasts at https://drive.google.com/drive/folders/10ozTBaSDtI-GnutEJK0qIzAFzyjLCVAN?usp=drive_link

2. https://github.com/aspiringsecurity/Inch-Care/tree/main/1inch-stellar-dapp/1inch-soroban-incident-mgmt (Stellar blockchain)

Demo and Screencasts at https://drive.google.com/drive/folders/1Fa9_YGTdKNVXAt-eL6IWxhTUXn2VRqDU?usp=drive_link



Contracts Deployment Addresses using 1inch fusion+ sdk

Ethereum Sepolia (Chain A)

- Deployer Address (Alice): 0x213064b9f671Bbe8b94C98283AE4D12CAB8E4f4C
- Escrow Contract: 0x3B469d926876f10cA002E5Cf20776745aAcDFd3A
- TokenA Contract: 0x7F1f595B7b47986b8B5a12731759225a2CcABfFC

Filecoin Calibration (Chain B1)
 
- Deployer Address (Bob): 0x08aDb9CC0658Bb91F57707B7B4D016312EF8c70a
- Escrow Contract: 0x6A6D7a69A302Ca8B41D7D00eD7019997854F587B
- TokenB Contract: 0x1114CC447697E1f981FD83107f3a65146aa918Cd

Starknet testnet (Chain B2)

- Starknet EscrowAddress: 0x00aa920d6d0f39225fea6e81e3b82193cbcc814c6b3541c6f6163ccf0fa1f5e4
- Starknet Utility Token Contract: 0x01d324a581d624d53b6b707092d1de5d7f4eba70546e94dee2d0367b9cbfa99b


Stellar Testnet Contract Link for Medical Incident Reporting and Management using 1inch fusion sdk+

Stellar deployed Contract (medical incident management):
https://stellar.expert/explorer/testnet/contract/CA5KTWZW6EK5HL4MAB7DXBYBIQZ7JQ3MAKH6UQXQL256P2I44PFR6MLS 

HTCL Contract (ETH): https://sepolia.etherscan.io/address/0x0ee168dff4412f271d483ea10fcd2b18fb57985a

Stellar transaction: https://sepolia.etherscan.io/tx/0xf588a26f0decf2edec42cd7197c08c7b008e632cfb8258fe6d6f5b6693191586 


