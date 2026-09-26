# PBG Pay — Holistic Permanent QR (INR)

**One QR → Pay in INR + Web3**

- **Permanent QR (PRINT THIS):** `https://drawdrawdraw2025.github.io/pbg-pay/`
- **This QR never changes.** It points to GitHub Pages, which loads `latest.json` → builds UPI string → shows dynamic UPI QR.
- **To change UPI ID / amount / name:** Edit `latest.json` → `git commit` → `git push` → done. No reprint.

**Bypasses:**
- No payment gateway (Razorpay/Paytm 2% fee) — direct UPI to bank
- No hosting/domain fees — GitHub Pages + Filebase IPFS (free)
- No ENS renewal for payments — QR is GitHub, ENS is optional for Web3 site

**latest.json**
```json
{
  "upi_id": "pbgmmindpower@upi",
  "payee_name": "PBG Mmindpower",
  "amount": "",   // "" = any, or "100" = fixed ₹100
  "currency": "INR",
  "note": "PBG Payment"
}
```

**Holistic:** This page also links to `https://drawdrawdraw2025.github.io/pbg-permanent/` (Web3 IPFS) and `https://pbgmmindpower.eth.limo` (ENS).

**Update without reprint:** Any change to `latest.json` instantly updates the inner UPI QR shown on the permanent page.
