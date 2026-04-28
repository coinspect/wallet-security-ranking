# Wallet Security Ranking - Data Repository

This is the data repository for the [Wallet Security Ranking](https://www.coinspect.com/wallets/) project. Stores the configuration, individual wallet reports, and historical ranking rounds that produce each published ranking.


## Repository Structure

```
/
├── config/                    # Current configuration (for upcoming rankings)
│   ├── categories.json
│   ├── wallets.json
│   └── checks.json
├── reports/                   # Latest reports (overwritten when re-tested)
├── scripts/                   # Automation scripts
├── YYYY-MM-DD/                # Test round folders by ISO date (e.g., 2025-12-31/)
│   ├── ranking.json
│   └── config/                # Configuration used for this round
│       ├── categories.json
│       ├── checks.json
│       └── wallets.json
├── CHANGELOG.md
```
## Contents
 
### `config/`
 
The **current** configuration that will be applied the next time a ranking is generated. Edits here affect upcoming rounds only; historical rounds keep their own snapshot (see below).
 
- `categories.json` - name, id, description, and weight for each security category evaluated
- `checks.json`  - security checks performed against each wallet
- `wallets.json` - name and URL for each wallet included in the ranking

#### `checks.json` format
 
Each entry is keyed by a versioned check ID (e.g. `WSR-PERM-001.v1`). A `~Mobile` / `~Browser` suffix is used when a check has separate variants per platform. For more information about these checks visit the [Wallet Security Benchmark](https://github.com/coinspect/wallet-security-framework/tree/main/WSB) repostiory. The WSB is a set of interaction-based security tests for web3 wallets that is part of the [Wallet Security Framework initiative.](https://github.com/coinspect/wallet-security-framework/)

### `reports/`
 
The latest security report for each wallet-platform combination. Files here are **overwritten** whenever a wallet is re-tested, so this folder always reflects the most recent state per wallet instead of the state at any specific ranking round. For point-in-time data, use the dated round folders below.
 
### `scripts/`
 
Automation scripts maintained alongside the data:
 
### `YYYY-MM-DD/`
 
Each completed ranking round is archived in a folder named after its ISO date (e.g. `2025-12-31/`). Round folders are **immutable snapshots**, so any past ranking can be reproduced from the data inside its own folder:
 
- `ranking.json` - full ranking results for the round
- `config/` - the config used for the round

### `CHANGELOG.md`
 
Notable changes to the Wallet Security Ranking data, including fixes of testing mistakes.
 
