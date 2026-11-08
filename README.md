# zuraffa-demo

Marketing demo target page for **Zuraffa Browser — on-device Translate Selection** (zuraffa_browser spec 590, PR #815).

**Live page:** https://arrrrny.github.io/zuraffa-demo/

A fictional Romanian checkout ("PrețulCorect.ro") that stages the marketing demo:

1. The Zuraffa scraper fleet hits the page's security verification (a Cloudflare Turnstile test widget + a Romanian question captcha).
2. `page_challenge_scan` detects the captcha → `notify_human` sends Ahmet a native macOS notification.
3. Ahmet taps the notification → the tab focuses → he sees the Romanian captcha ("opt + patru = ?").
4. He selects the Romanian text → right-click → **Translate Selection** → the on-device Apple Translation engine renders English. No cloud, no service call.
5. He types the answer (`12`) → "Verificare reușită!" → captcha solved, checkout continues.

Everything on the page is fictional (store, prices, phone, address). The Turnstile sitekey is Cloudflare's always-pass test key (`1x00000000000000000000AA`). The answer to the captcha is `12`.
