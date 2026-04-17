# Futures Foundations Course Website + Curriculum Pack

This repo now includes a full beginner futures course package and a sell-ready website.

## What's Included

- **Public website** (`site/`) with:
  - Landing page
  - Curriculum page
  - 8 chapter lesson pages
  - Stripe-ready checkout page
  - Payment success page
- **Course operations pack** (`course/`) with:
  - Master curriculum document
  - Sales page copy
  - Video scripts for all 8 chapters
  - Quizzes + answer keys for all 8 chapters
  - Slide outlines for all 8 chapters

## Quick Start (Local)

```bash
cd /workspace/futures-course-site
python3 -m http.server 8000 --directory site
```

Then visit: `http://localhost:8000`

## Connect Payments (Stripe)

1. Create a product in Stripe dashboard.
2. Create a payment link or Checkout Session endpoint.
3. Replace checkout link in `site/checkout.html`:
   - `https://buy.stripe.com/test_replace_with_your_link`
4. Set post-payment redirect to `/success.html`.

## Deploy in Minutes

### Option A: Netlify
1. Create new site from this repo.
2. Set publish directory to `site`.
3. Deploy.

### Option B: Vercel
1. Import repo.
2. Set output directory to `site` (static hosting).
3. Deploy.

### Option C: AWS S3 + CloudFront
1. Upload `site/` as static website files.
2. Add CloudFront + HTTPS.

## Important Compliance Note

This course is educational only and does not provide investment advice or guaranteed returns.

## Suggested Immediate Next Steps to Sell

1. Record chapter videos using scripts in `course/video-scripts/`.
2. Upload videos to your course host (Kajabi/Thinkific/Teachable/Gumroad + unlisted video).
3. Point your domain to hosted `site/`.
4. Run traffic to landing page and checkout.
