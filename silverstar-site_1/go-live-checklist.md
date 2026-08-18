# Silver Star Detailing — Go-Live Checklist

Everything left to take this from "finished file" to "published, working website." Rough time and cost estimates included so you can price the job and set expectations with the client.

## 1. Activate the quote form (5 minutes, free)

The contact form is already wired to send email via FormSubmit — no backend needed — but it's pointed at a placeholder address.

- [ ] Decide which inbox should receive quote requests (David's personal email is fine to start; a real business inbox can come later).
- [ ] Open `index.html`, find `QUOTE_FORM_EMAIL` near the bottom of the file, and replace the placeholder with that real address.
- [ ] Submit the form once yourself after publishing. FormSubmit sends a one-time confirmation email to that inbox — someone has to click the link in it before requests start arriving normally. Do this step yourself so it's already activated before the client sees the site.
- [ ] Send a second test submission after confirming, to make sure it actually lands in the inbox (check spam folder too).

## 2. Buy a domain ($10–$20/year)

- [ ] Pick a domain — `silverstardetailing.com` or similar, through any registrar (Namecheap, Google Domains successor Squarespace Domains, Cloudflare Registrar, GoDaddy).
- [ ] This cost is normally passed through to the client, not absorbed into your build fee — call it out as a separate line item.

## 3. Host the site (free–$5/month)

Pick one:

- [ ] **Netlify or Vercel** (recommended) — free tier, drag-and-drop deploy of the `index.html` + `assets` folder, automatic HTTPS, easy custom-domain connection. Best option for a static site like this one.
- [ ] **GitHub Pages** — free, works well if you're comfortable with git, slightly more setup for a custom domain.
- [ ] **Traditional shared hosting** (Bluehost, SiteGround, etc.) — usually $3–$10/month, only worth it if the client also wants business email hosted there (e.g. `hello@silverstardetailing.com`).

## 4. Connect the domain to the host (15–30 minutes)

- [ ] Point the domain's DNS at the host (each host gives exact instructions — usually adding an A record or changing nameservers).
- [ ] Wait for DNS propagation (can take a few minutes to a few hours).
- [ ] Confirm HTTPS/SSL is active (Netlify/Vercel/GitHub Pages do this automatically and for free).

## 5. Set up business email (optional, $0–$6/user/month)

Only needed if the client wants `@silverstardetailing.com` addresses instead of a personal Gmail:

- [ ] Google Workspace or Zoho Mail (Zoho has a free tier for a single user) both work well with a domain bought elsewhere.
- [ ] Update `QUOTE_FORM_EMAIL` in the form script to the new business address once it's live.

## 6. Real content pass (scope this separately — it's real work)

Still placeholder right now:

- [ ] Before/after photos (currently placeholder graphics)
- [ ] Owner/team photo in the About section
- [ ] Testimonials (currently sample reviews, not real ones)
- [ ] Confirm business hours and service list are accurate

## 7. Final test before sending the link to the client

- [ ] Open the live URL on an actual phone and test the before/after slider with your finger.
- [ ] Submit the quote form for real and confirm the email arrives.
- [ ] Tap the phone number, email, and "Get Directions" links on a phone to confirm they open the dialer, mail app, and Maps.
- [ ] Check the site on both light-background and dark-background phone screenshots (some phones auto-invert or apply dark mode filters) — not required, just worth a glance.

---

**Rough total cost to get this live (excluding your labor):** $10–$30/year for the domain, $0/month for hosting on Netlify/Vercel, $0–$6/month if business email is added. Everything else is your time.
