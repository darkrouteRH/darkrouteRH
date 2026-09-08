<div align="center">

<img src="https://darkroute.exchange/logo.png" alt="DarkRoute" width="140" />

# DarkRoute

### Swap in the dark. Know exactly where it went.

Private, non-custodial swap routing on **Robinhood Chain**.
No account. No KYC. A receipt that names the venue and prints the fee.

[**Launch app**](https://app.darkroute.exchange) · [Website](https://darkroute.exchange) · [Docs](https://app.darkroute.exchange/docs) · [X](https://x.com/DarkrouteRH)

</div>

---

## The problem

Private swapping is a real need with a dishonest supply.

Open any private swapper today. It shows you a wall of nineteen exchange logos, fills your order through three partner APIs, prints a household exchange name that had nothing to do with it, and never tells you what it charged.

DarkRoute takes the opposite side: **hide the order from the market, never hide the mechanics from the user.**

---

## Live now

The router is open and settling real swaps today — no waitlist, no wallet connect, no signup.

| | |
|---|---|
| **Real routing** | Live quotes across **188 assets on 35 chains**. The venue filling your order is named as-is — never relabeled. |
| **Non-custodial orders** | Every order returns a real one-time deposit address + QR. Funds go straight into the route; DarkRoute never holds them. |
| **Live status tracking** | Awaiting deposit → Confirming → Exchanging → Settled, polled server-side and pushed to the page. |
| **Shareable receipts** | Route, venue, fee and settlement in one card. The receipt is the product. |
| **Wallet sign-in** | EVM `personal_sign` over a server nonce. No approvals, no transactions, no gas — the signature only proves you hold the key. |
| **Rewards ledger** | Per-address swap history, 30-day volume, and live cashback ladder progress. |
| **0% fee during beta** | The DarkRoute fee is printed at its 0.3% reference rate and **not charged** while the fee vault is being built. You pay the venue's 0.1% and nothing else. |
| **Docs** | Including a plain-words page on exactly what "private" does and does not mean. |

Try it → **[app.darkroute.exchange](https://app.darkroute.exchange)**

---

## How one swap works

```
1  Pick send + receive          no wallet connect, no signup
2  Quote                        venue named as-is, fee printed before you deposit
3  Paste receiving address      network inferred from the address shape
4  Deposit                      one-time address + QR, straight into the route
5  Track                        Awaiting → Confirming → Exchanging → Settled
6  Receipt                      venue, fee, settlement — shareable
```

Typical settle time is 5 to 30 minutes.

---

## What "private" actually means

We would rather print the limits than get caught having hidden them.

**Hidden from the market**
- Your order never touches a public order book or the mempool as a visible swap.
- No account links your swaps together. Only the receiving address is known to the route.

**Not hidden — and we say so**
- The venue filling your order sees the deposit and the receiving address. That is how non-custodial works.
- On-chain settlement is public, because chains are public.
- We keep an order record for support and rewards. No names, no emails, no KYC.

Overclaiming privacy is how this category loses trust.

---

## Shipping next

- **Multi-venue route table** — instant-exchange partners and native Robinhood Chain pools alongside the current intent leg, so the quote lists every venue that actually quoted
- **Fee vault + cashback settler** on Robinhood Chain — turns the printed 0.3% on, and starts paying cashback in tokenized stocks with a settlement hash
- **Dark Split** — one order across several venues, sized to each venue's real depth, so no single venue sees the full size
- **Agent desk** — an autonomous trading desk with a public wallet and hard-coded rails, mirrorable into your own wallet
- **Public API** — `/v1/quote` and `/v1/order`, the same route table the app shows
- **Limit + DCA orders**, portfolio, launch tab

---

## $DARK

**$DARK has not launched.** There is no contract address yet.

Any token claiming to be $DARK right now is fake. The contract will be announced **only** from [@DarkrouteRH](https://x.com/DarkrouteRH), and nowhere else.

When it does launch, it will be a fair launch on the pons v2 launchpad — 1,000,000,000 supply, **zero team allocation**, no presale, no unlock cliffs. The token buys cheaper fees and access to power features. It never buys a better route: route quality and venue honesty are identical for everyone, holder or not.

---

## Stack

Next.js 16 · TypeScript · Tailwind 4 · Postgres with forced row-level security · Docker behind Traefik

Containers run non-root, secrets never reach the browser bundle, and every write endpoint fails closed.

---

<div align="center">

**[darkroute.exchange](https://darkroute.exchange)** · **[app.darkroute.exchange](https://app.darkroute.exchange)**

[X](https://x.com/DarkrouteRH) · [Docs](https://app.darkroute.exchange/docs)

<sub>DarkRoute is a non-custodial routing interface. It does not hold user funds, does not provide investment advice, and does not guarantee execution, rates, or settlement times, which depend on third-party venues and network conditions. Crypto assets are volatile and transactions are irreversible — verify the receiving address and network before every swap. "Private" refers to order routing away from public order books; venues and public blockchains retain their own visibility. Never risk funds you cannot afford to lose.</sub>

</div>
