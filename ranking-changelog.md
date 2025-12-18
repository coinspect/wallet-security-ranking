---
title: Wallet Ranking Changelog
background: scoring-hero.png
excerpt: "Track the corrections and improvements made across different versions of our Wallet Security Ranking. We are committed to transparency and continuous improvement."
socialImage: wallet-ranking-testing-social-image.png
release-version: "3"
release-date: "Nov 21, 2025"
versions:
  - date: "Current Release"
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
                reason: "Wrong Result - Data entry error (inverted result)."
          - name: "Phantom"
            changes:
              - check: "Disables eth_sign method"
                change: "0 → 100"
                reason: "Wrong Result - Data entry error (inverted result)."
          - name: "Rainbow"
            changes:
              - check: "Clear interface for ERC20 Approve / Automatic Wallet Lock"
                change: "100 → 0"
                reason: "Wrong Result - Data entry error (inverted result)."
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
                reason: "Incorrect Result - Data entry error (inverted result)."
          - name: "imToken"
            changes:
              - check: "Robust Authentication"
                change: "100 → 0"
                reason: "Incorrect Result - Data entry error (inverted result)."
          - name: "MetaMask"
            changes:
              - check: "Alerts on phishing DApps"
                change: "0 → 100"
                reason: "Testing Error - Confusion regarding description. Works on the Embedded Browser."
          - name: "Okto"
            changes:
              - check: "Verified URLs"
                change: "100 → 0"
                reason: "Incorrect Result - Data entry error (inverted result)."
          - name: "Rabby Wallet"
            changes:
              - check: "dApp Connection Information"
                change: "100 → 0"
                reason: "Incorrect Result - Data entry error (inverted result)."
          - name: "Trust Wallet"
            changes:
              - check: "Verified URLs"
                change: "100 → 0"
                reason: "Incorrect Result - Data entry error (inverted result)."
          - name: "Uniswap"
            changes:
              - check: "Alerts on phishing addresses / Interacting with an unknown Address"
                change: "0 → 100"
                reason: "Incorrect Result - Data entry error (inverted result)."
          - name: "Zerion"
            changes:
              - check: "Alerts on phishing addresses"
                change: "0 → 100"
                reason: "Incorrect Result - Data entry error (inverted result)."
---

## Understanding the Corrections

- **Incorrect Result:** The check was correctly tested, but the selected score was inverted (e.g., marked as Pass instead of Fail).
- **Testing Error:** The feature location was missed, or there was confusion regarding the check mechanics during the initial test.
