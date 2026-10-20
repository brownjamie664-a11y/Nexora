# NEXORA — GitHub Pages website

## Launch for free
1. Sign in at github.com and create a **public** repository named `nexora` (or another available name).
2. Upload `index.html` into the root of the repository and commit it.
3. Go to **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, branch **main**, folder **/(root)**, then Save.
4. Wait for GitHub Pages to deploy. The URL should be `https://YOUR-USERNAME.github.io/nexora/` (substitute your username and repository name).

## Enable real payments
1. Create and verify your own Stripe account at stripe.com.
2. Create three **one-time payment** products at EUR 249, EUR 599, EUR 999. Clearly specify what's included, delivery arrangements, and your refund/cancellation policy before accepting payment.
3. For each product, create a Stripe **Payment Link**. Configure receipt and post-purchase information in Stripe. Ensure the checkout collects enough customer contact information and set up an onboarding follow-up process.
4. In `index.html`, find `const STRIPE_LINKS={starter:'',business:'',premium:''};` and paste each matching `https://buy.stripe.com/...` URL between the quotes. Commit the updated file. The buttons automatically become **Pay securely**.
5. Test each link and checkout configuration before sending traffic. Never place Stripe secret API keys in GitHub Pages code.

**Important:** Until links are supplied, checkout buttons intentionally say “Checkout coming soon” and do not accept money. Stripe processing fees apply. GitHub Pages hosting is free for eligible public repositories, but domain purchases and third-party services may cost money.

## Before taking orders
- Confirm NEXORA name availability, including business name and trademarks.
- Add accurate business identity and contact information and publish terms, privacy and refund/cancellation policies appropriate to your location.
- Confirm your capacity to deliver packages and communicate timelines clearly.
- Add a working customer onboarding/contact route after payment.
- The three portfolio examples are illustrative concepts, not real customer testimonials or work.
