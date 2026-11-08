# is this link a scam?

Paste a link, or the whole message you got, before you click anything. The page never opens the link.

**Live:** https://cranefomo.github.io/isitascam

## What it checks

| Check | Source |
|---|---|
| Known scam domains (230k+, incl. crypto drainers). Confirmed scams and community reports are shown separately | [PhishDestroy DestroyList](https://github.com/phishdestroy/destroylist), which also aggregates MetaMask, ScamSniffer, SEAL, Polkadot, OpenPhish, URLhaus, Phishing.Database and more |
| Malware / phishing filter | Cloudflare malware-filtering DNS (1.1.1.2) |
| Domain age and registrar | public RDAP registration records via [rdap.org](https://rdap.org) |
| Site popularity | [Tranco](https://tranco-list.eu) top 1M sites list |
| Look-alike tricks the databases may not have yet | built in, runs in your browser |

Look-alike checks:
- fake brand domains (`metamask-wallet-restore.com`, `pump-fun-claim.xyz`) across 100+ brands: wallets, exchanges, DeFi, delivery, banks
- misspellings (`ledgr-live.pages.dev`, `krakden.com`, `coinbsae.com`, `rnetamask` with "rn" for "m")
- Cyrillic or Greek letters that look like Latin ones
- the `@` trick (`https://binance.com@scam.site` goes to `scam.site`)
- a real name at the start (`binance.com.verify-login.xyz`)
- short links that hide the destination, with a link to the shortener's own preview page
- free site builders (vercel.app, pages.dev, weebly) and real platforms where anyone can post (Google Forms, Telegram, Discord)
- scam words (claim, airdrop, verify, restore, seed) and cheap domain zones

You can paste a whole DM: every link in it is found and checked one by one.

## Privacy

- The link is never opened.
- Only the domain name (no path, no tokens) is sent to the services above.
- No trackers, no cookies, nothing is saved.

## Tested

- 259 legit sites (top sites, banks, exchanges, wallets, DeFi, Ukrainian services): no false scam verdicts except one domain that community blocklists themselves report.
- 150 random live scam domains from the database: 150 flagged.
- Local look-alike checks alone (no database) catch about 22% of 2,000 real scam domains. The database does the rest.
- Script injection, broken input, offline services: handled, an error is never shown as "safe".

## Limits

"No red flags" does not mean safe. A brand-new scam may not be in any list yet, and some zones (like `.io`) don't publish registration dates.

## Credits

Scam data: PhishDestroy DestroyList (MIT). Not affiliated with any of the services above.

Built by [@Cranefomo](https://x.com/Cranefomo).

## No token

This project has no token or coin. Any coin using this name is not created or endorsed by me.
