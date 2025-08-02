# Medical Incident Reporting on Stellar & EVM

This project enables decentralized reporting of medical incidents and processing of insurance payments across both **Stellar/Soroban** and **EVM-compatible blockchains** using the **1inch Fusion SDK+**.

We leverage:

* **Soroban smart contracts** on the Stellar blockchain for secure, immutable medical incident logs.
* **1inch Fusion+** for routing payments and cross-chain insurance claims via decentralized settlement protocols.

---

## 🚑 Use Case

**For Hospitals, Insurers & Aid Organizations**

* **Report** medical incidents on-chain (Soroban)
* **Verify** and timestamp reports immutably
* **Trigger** insurance claim fulfillment using EVM-compatible smart contracts
* **Execute** cross-chain payments with Fusion+ (e.g., from Stellar to Ethereum or Polygon)

---

## 🧱 Project Structure

This repository follows the recommended structure for Soroban contracts:

```text
.
├── contracts
│   └── incident_report
│       ├── src
│       │   ├── lib.rs         # Soroban smart contract for incident logging
│       │   └── test.rs        # Unit tests for the Soroban contract
│       └── Cargo.toml         # Local dependencies for the contract
├── scripts
│   └── fusion_swap.ts         # Cross-chain payment script using 1inch Fusion SDK+
├── frontend
│   └── ...                    # Optional web interface for hospitals/NGOs
├── Cargo.toml                 # Workspace file for dependencies
└── README.md
```

---

## 🧪 Components

### `incident_report` (Soroban Contract)

* Logs medical events immutably
* Supports structured metadata (e.g., patient ID hash, event type, timestamp)
* Emits events for integration with oracles or EVM listeners

### `fusion_swap.ts` (1inch Fusion+ Script)

* Facilitates settlement of insurance claims across chains
* Uses hashlock/timelock logic for conditional transfers
* Integrates EVM smart contract with Soroban triggers


## 📡 Fusion+ Integration

Ensure you have:

* Access to 1inch Fusion SDK+
* Private key and relayer rights (if using resolvers)
* EVM-compatible wallet with testnet funds

```ts
// Example: Cross-chain swap from Stellar to Polygon
await executeCrossChainSwap({
  fromChain: 'stellar',
  toChain: 'polygon',
  amount: '1000',
  takerAddress: '<insured_party>',
  secretHash: '<hashlock>'
});
```

---

## 💡 Future Roadmap

* [ ] Add patient consent registry
* [ ] Enable claim adjudication DAO
* [ ] Launch frontend for hospital reporting
* [ ] Interoperability with FHIR/EHR systems


## 📜 License

MIT

