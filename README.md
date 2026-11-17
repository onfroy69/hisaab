# Hisaab 💬🧾 — Bunty Kirana Store

A simple digital ledger for a local shop — like the notebook a kirana keeps for who owes what, with a WhatsApp reminder in one tap.

**Live app:** https://onfroy69.github.io/hisaab/

## Features

- Add customers (name + 10-digit phone) and entries (credit / payment with amount, date, note)
- Per-customer balance & shop total outstanding at the top
- Customer ledger page, newest entries first
- Payment screenshots attached to entries (compressed & stored locally)
- **Automatic amount reading from screenshots** — OCR reads the number after the ₹ symbol and fills the amount box
- One-tap polite WhatsApp reminder with customer name, balance in rupees and a UPI pay link (`upi://pay?pa=karkakarthik@ybl` / https://upi.pe/karkakarthik@ybl)
- Data persists in browser storage (localStorage) — no database, no AI
- Import box for shop JSON (`#import-box` + `#import-go`)
- Honours `?today=YYYY-MM-DD` reference date
- Bonus: overdue list sorted by days since last payment, edit & delete entries with live recalculation, CSV export, search by name/phone, UPI pay link in reminders, Hindi / Telugu / English labels, dark & light mode
- Mobile-first, built for 375 px screens

## Testing

Load `sample-data.json` via the import box (📥 button). With reference date `?today=2026-11-15` the shop total should be **Rs 11,820** across 8 customers, matching `sample-expected.json`.
