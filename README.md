# Invest Money - Smart Crypto Investment Platform

A modern investment platform built with vanilla HTML/CSS/JS that allows users to deposit USDT (TRC20/BEP20/ERC20), invest in fixed-return plans, claim daily profits, and withdraw.

## Features

- **5 Investment Plans**: Bronze ($100), Silver ($200), Gold ($400), Platinum ($800), Diamond ($1,600) - 60 days duration
- **Daily Profit Claim**: Each plan has independent claim with 24h cooldown
- **Admin Panel**: Hidden access with TOTP (Google Authenticator) + Email Verification
- **Deposit/Withdraw**: TRC20, BEP20, ERC20 networks supported
- **Transfer**: Move profit to deposit balance for reinvestment
- **Backup/Restore**: Export and import user data as JSON
- **Legal Pages**: Terms, Privacy, Risk Disclosure, AML/KYC, Refund Policy
- **PWA**: Installable on mobile
- **Supabase**: Hybrid mode (Cloud + localStorage fallback)
- **Push Notifications**: Browser native
- **Telegram Bot**: Admin notifications
- **Email Service**: SMTP for OTP and notifications
- **Google Analytics**: Event tracking ready

## Tech Stack

- **Frontend**: Pure HTML, CSS, JavaScript (no framework)
- **Storage**: localStorage + Supabase PostgreSQL (hybrid)
- **Charts**: SVG-based custom charts
- **TOTP**: RFC 6238 implementation with Web Crypto API
- **PWA**: Service Worker + Manifest

## Deployment

### Vercel (Recommended)

1. Push this repository to GitHub
2. Import to Vercel: https://vercel.com/new
3. Vercel will auto-detect static site and deploy
4. Add custom domain in Settings → Domains

### Local Development

Just open `index.html` in a modern browser (Chrome recommended).
For full PWA features, serve over HTTPS.

## Admin Access

The admin login is hidden by default. Access via:
- URL: `?admin=true`
- Keyboard: `Ctrl+Shift+A`
- Type "secret" anywhere

Default credentials:
- Username: `admin`
- Password: `admin123`

**IMPORTANT**: Change these immediately after first login via Settings → Admin Credentials.

## License

Proprietary - All Rights Reserved