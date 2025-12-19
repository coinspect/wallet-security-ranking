---
title: Wallet Ranking Changelog
background: scoring-hero.png
excerpt: "Track the corrections and improvements made across different versions of our Wallet Security Ranking. We are committed to transparency and continuous improvement."
socialImage: wallet-ranking-testing-social-image.png
release-version: "3"
release-date: "Nov 21, 2025"
versions:
  - date: "Dec 19, 2025 (Current Release)"
    platforms:
      - name: "Android"
        vendors:
          - name: "OKX"
            changes:
              - check: "Parses EIP-712 objects"
                change: "0 → 100"
                reason: "Testing Error - Initially failed, but subsequently verified working using a USDC ERC-20 permit."
      - name: "Extension (Browser)"
        vendors:
          - name: "OKX"
            changes:
              - check: "Automatic Wallet Lock"
                change: "100 → 0"
                reason: "**Data entry error**: Tester selected the wrong score."
          - name: "Phantom"
            changes:
              - check: "Disables eth_sign method"
                change: "0 → 100"
                reason: "**Data entry error**: Tester selected the wrong score."
          - name: "Rainbow"
            changes:
              - check: "Clear interface for ERC20 Approve / Automatic Wallet Lock"
                change: "100 → 0"
                reason: "**Data entry error**: Tester selected the wrong score."

  - date: "Dec 03, 2025"
    platforms:
      - name: "Android"
        vendors:
          - name: "imToken"
            changes:
              - check: "Alerts on phishing DApps"
                change: "0 → 100"
                reason: "Testing Error - The initial dApp used did not trigger the warning. Re-testing with a different dApp successfully triggered the alert."
          - name: "MetaMask"
            changes:
              - check: "List and revoke token approvals"
                change: "0 → 100"
                reason: "Testing Error - Feature was initially missed. Located in Browser > Connect > Dashboard > Spending Caps."
              - check: "Alerts on phishing DApps"
                change: "0 → 100"
                reason: "Testing Error - Confusion regarding the check description. Works on Embedded Browser (not via WalletConnect)."
      - name: "iOS"
        vendors:
          - name: "Coin Wallet"
            changes:
              - check: "Different ChainID"
                change: "0 → 100"
                reason: "**Data entry error**: Tester selected the wrong score."
          - name: "imToken"
            changes:
              - check: "Robust Authentication"
                change: "100 → 0"
                reason: "**Data entry error**: Tester selected the wrong score."
          - name: "MetaMask"
            changes:
              - check: "Alerts on phishing DApps"
                change: "0 → 100"
                reason: "Testing Error - Confusion regarding description. Works on the Embedded Browser."
          - name: "Okto"
            changes:
              - check: "Verified URLs"
                change: "100 → 0"
                reason: "**Data entry error**: Tester selected the wrong score."
          - name: "Rabby Wallet"
            changes:
              - check: "dApp Connection Information"
                change: "100 → 0"
                reason: "**Data entry error**: Tester selected the wrong score."
          - name: "Trust Wallet"
            changes:
              - check: "Verified URLs"
                change: "100 → 0"
                reason: "**Data entry error**: Tester selected the wrong score."
          - name: "Uniswap"
            changes:
              - check: "Alerts on phishing addresses / Interacting with an unknown Address"
                change: "0 → 100"
                reason: "**Data entry error**: Tester selected the wrong score."
          - name: "Zerion"
            changes:
              - check: "Alerts on phishing addresses"
                change: "0 → 100"
                reason: "**Data entry error**: Tester selected the wrong score."

  - date: "Nov 21, 2025 (Initial Release)"
    platforms:
      - name: "Extension (Browser)"
        vendors:
          - name: "NuFi"
            changes:
              - check: "Included in evaluation pool"
                change: "0 → 100"
                reason: "Added to the wallet ranking to expand browser extension coverage and share testing results with the WalletBeat initiative."
          - name: "Elytro"
            changes:
              - check: "Included in evaluation pool"
                change: "0 → 100"
                reason: "Added as a browser extension wallet as part of our commitment to transparently share testing results with the WalletBeat initiative."
          - name: "Taho"
            changes:
              - check: "Eligibility for evaluation"
                change: "0 → 100"
                reason: "Excluded due to inactivity. The extension was last updated on April 18, 2025, which falls outside our freshness threshold relative to the March 26, 2025 ranking baseline."
          - name: "BlockWallet"
            changes:
              - check: "Eligibility for evaluation"
                change: "100 → 0"
                reason: "Discontinued. The project has officially announced a sunset effective January 1, 2026, and is no longer maintained."
      - name: "iOS"
        vendors:
          - name: "Daimo"
            changes:
              - check: "Eligibility for evaluation"
                change: "0 → 0"
                reason: "Excluded. The iOS application was not available for download during the testing window, likely due to geofencing or temporary delisting."
          - name: "Ambire"
            changes:
              - check: "Eligibility for evaluation"
                change: "100 → 0"
                reason: "Excluded. The iOS application is currently not available for public download."
      - name: "Android"
        vendors:
          - name: "Family"
            changes:
              - check: "Eligibility for evaluation"
                change: "0 → 0"
                reason: "Excluded. No Android version exists; the wallet is currently iOS-exclusive."
      - name: "Mobile"
        vendors:
          - name: "Clave"
            changes:
              - check: "Eligibility for evaluation"
                change: "0 → 0"
                reason: "Excluded. While supporting Arbitrum One and Base, the wallet lacks a dApp browser and WalletConnect support, preventing full evaluation under standard criteria."
          - name: "AlphaWallet"
            changes:
              - check: "Eligibility for evaluation"
                change: "100 → 0"
                reason: "Excluded. The mobile application is no longer available for download via standard app stores."
          - name: "Privy"
            changes:
              - check: "Eligibility for evaluation"
                change: "0 → 0"
                reason: "Excluded. Confirmed to operate as a wallet infrastructure provider (WaaS) for developers rather than a standalone consumer wallet."

---

## Understanding the Corrections

- **Incorrect Result:** The check was correctly tested, but the selected score was inverted (e.g., marked as Pass instead of Fail).
- **Testing Error:** The feature location was missed, or there was confusion regarding the check mechanics during the initial test.

