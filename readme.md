# Learnly — Educational Website

## Files included
- `index.html` — Landing page (marketing site)
- `signup.html` — 4-step signup flow (parent account → child profile → plan → done)
- `login.html` — Login page
- `app.html` — Main dashboard (post-login)

## Pricing (ZAR)
- Free: R0/month — 1 child, limited lessons
- Family: R100/month — up to 4 kids, all subjects, parent dashboard
- School: R300/month — unlimited learners, teacher dashboard, CAPS aligned

---

## How to publish this as a real website

### Option 1: Netlify (easiest — free hosting)
1. Go to https://netlify.com and create a free account
2. Drag and drop the entire `learnly` folder onto the Netlify dashboard
3. Your site goes live instantly at a URL like `learnly.netlify.app`
4. To use your own domain (e.g. learnly.co.za), go to Domain Settings and follow the steps

### Option 2: Vercel (also free)
1. Go to https://vercel.com and sign up
2. Install Vercel CLI: `npm install -g vercel`
3. In this folder, run: `vercel`
4. Follow the prompts — your site is live in seconds

### Option 3: GitHub Pages (free)
1. Create a GitHub account at https://github.com
2. Create a new repository named `learnly`
3. Upload all files to the repository
4. Go to Settings → Pages → set source to `main` branch
5. Your site goes live at `yourusername.github.io/learnly`

---

## Getting a South African domain
- Register `.co.za` at https://domains.co.za or https://afrihost.com
- Typical cost: R60–R120/year for a .co.za domain
- After registering, point the domain to your Netlify/Vercel site using their DNS instructions

---

## Next steps to make it fully functional
1. **Authentication** — Add Firebase Auth (free tier) for real login/signup
   - https://firebase.google.com
2. **Database** — Firebase Firestore to store user progress and XP
3. **Payments** — Add PayFast (South African payment gateway) for subscriptions
   - https://payfast.io — supports EFT, credit card, Instant EFT
4. **Content** — Add actual lesson content and quiz pages
5. **Email** — Use Mailgun or SendGrid to send welcome/progress emails

---

## PayFast integration (South African payments)
PayFast is the best payment gateway for South African Rand subscriptions.
- Supports: Credit/Debit card, EFT, Instant EFT, Snapscan, Mobicred
- Monthly subscriptions for R100 (Family) and R300 (School)
- Sign up at https://payfast.io and follow their subscription API docs
