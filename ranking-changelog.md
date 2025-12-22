---
title: Wallet Ranking Changelog
background: scoring-hero.png
excerpt: "A transparent record of how our Wallet Security Rankings evolve"
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
                        reason: "This was a testing error, where initially failed, but subsequently verified working using a USDC ERC-20 permit."
          - name: "Extension (Browser)"
            vendors:
                - name: "OKX"
                  changes:
                      - check: "Automatic Wallet Lock"
                        change: "100 → 0"
                        reason: "The tester mistakenly selected the wrong score."
                - name: "Phantom"
                  changes:
                      - check: "Disables eth_sign method"
                        change: "0 → 100"
                        reason: "The tester mistakenly selected the wrong score."
                - name: "Rainbow"
                  changes:
                      - check: "Clear interface for ERC20 Approve / Automatic Wallet Lock"
                        change: "100 → 0"
                        reason: "The tester mistakenly selected the wrong score."

    - date: "Dec 03, 2025"
      platforms:
          - name: "Android"
            vendors:
                - name: "imToken"
                  changes:
                      - check: "Alerts on phishing DApps"
                        change: "0 → 100"
                        reason: "Initially, the dApp used did not trigger any warnings. Re-testing with a different dApp successfully triggered the alert."
                - name: "MetaMask"
                  changes:
                      - check: "List and revoke token approvals"
                        change: "0 → 100"
                        reason: "This feature was initially missed. The feature is located in Browser > Connect > Dashboard > Spending Caps."
                      - check: "Alerts on phishing DApps"
                        change: "0 → 100"
                        reason: "There was a confusion regarding the check description. This feature works on Embedded Browser (but not via WalletConnect)."
          - name: "iOS"
            vendors:
                - name: "Coin Wallet"
                  changes:
                      - check: "Different ChainID"
                        change: "0 → 100"
                        reason: "The tester mistakenly selected the wrong score."
                - name: "imToken"
                  changes:
                      - check: "Robust Authentication"
                        change: "100 → 0"
                        reason: "The tester mistakenly selected the wrong score."
                - name: "MetaMask"
                  changes:
                      - check: "Alerts on phishing DApps"
                        change: "0 → 100"
                        reason: "There was a confusion regarding check description. Works on the Embedded Browser."
                - name: "Okto"
                  changes:
                      - check: "Verified URLs"
                        change: "100 → 0"
                        reason: "The tester mistakenly selected the wrong score."
                - name: "Rabby Wallet"
                  changes:
                      - check: "dApp Connection Information"
                        change: "100 → 0"
                        reason: "The tester mistakenly selected the wrong score."
                - name: "Trust Wallet"
                  changes:
                      - check: "Verified URLs"
                        change: "100 → 0"
                        reason: "The tester mistakenly selected the wrong score."
                - name: "Uniswap"
                  changes:
                      - check: "Alerts on phishing addresses / Interacting with an unknown Address"
                        change: "0 → 100"
                        reason: "The tester mistakenly selected the wrong score."
                - name: "Zerion"
                  changes:
                      - check: "Alerts on phishing addresses"
                        change: "0 → 100"
                        reason: "The tester mistakenly selected the wrong score."

eligibility_changes:
    - date: "Nov 21, 2025"
      added:
          - name: "NuFi"
            platform: "Extension (Browser)"
            reason: "Added to the wallet ranking to expand browser extension coverage and share testing results with the WalletBeat initiative."
          - name: "Elytro"
            platform: "Extension (Browser)"
            reason: "Added as a browser extension wallet as part of our commitment to transparently share testing results with the WalletBeat initiative."

      removed:
          - name: "BlockWallet"
            platform: "Extension (Browser)"
            reason: "The project has officially announced a sunset effective January 1, 2026, and is no longer maintained."
          - name: "Ambire"
            platform: "iOS"
            reason: "The iOS application is currently not available for public download."
          - name: "AlphaWallet"
            platform: "Mobile"
            reason: "The mobile application is no longer available for download via standard app stores."

    - date: "Apr 18, 2025"
      added:
          - name: "Ambire"
            platform: "Extension (Browser)"
            reason: ""
          - name: "Binance"
            platform: "Mobile"
            reason: ""
          - name: "Brave"
            platform: "Extension (Browser)"
            reason: ""
          - name: "Coin98"
            platform: "Extension (Browser)"
            reason: ""
          - name: "Ctrl Wallet"
            platform: "Extension/Mobile"
            reason: ""
          - name: "Family"
            platform: "iOS"
            reason: ""
          - name: "OKX"
            platform: "Mobile"
            reason: ""
          - name: "Okto"
            platform: "Mobile"
            reason: ""
          - name: "Tomo"
            platform: "Extension/Mobile"
            reason: ""

      removed:
          - name: "AlphaWallet"
            platform: "iOS"
            reason: ""
          - name: "Aurox Wallet"
            platform: "Extension (Browser)"
            reason: ""
          - name: "Loopring Wallet"
            platform: "Mobile"
            reason: ""
          - name: "ShapeShift"
            platform: "Mobile"
            reason: ""
          - name: "xDefi Wallet"
            platform: "Extension (Browser)"
            reason: ""
    - date: "Oct 25, 2024"
      note: "Initial release of Wallet Security Rankings"
---

### Updates may reflect testing refinements, data entry corrections, or clarified feature behavior identified during re-verification.
