# GlowPick — Fashion & Beauty Affiliate Site

## Your folder structure
```
glowpick/
├── public/
│   ├── index.html     ← your website
│   └── blogs.json     ← ADD YOUR POSTS HERE
└── vercel.json        ← Vercel config (don't touch)
```

---

## How to add a new blog post

Open `public/blogs.json` and add a new entry like this:

```json
{
  "id": 7,
  "title": "YOUR PINTEREST POST TITLE",
  "description": "Copy your Pinterest caption / write your blog description here. The more detail the better — talk about why you love the product.",
  "pinImage": "PASTE YOUR PINTEREST IMAGE URL HERE",
  "pinterestUrl": "https://www.pinterest.com/pin/YOUR-PIN-ID",
  "category": "Skincare",
  "date": "March 2026",
  "tags": ["skincare", "glow", "serum"],
  "amazon": {
    "productName": "Product Name from Amazon",
    "productImage": "AMAZON PRODUCT IMAGE URL",
    "price": "₹599",
    "originalPrice": "₹899",
    "rating": "4.3",
    "reviews": "12,483",
    "affiliateUrl": "https://amzn.to/YOUR-AFFILIATE-LINK"
  }
}
```

### Getting each piece of info:

**pinImage** (Pinterest image URL):
1. Open your Pinterest pin
2. Right-click the image → "Open image in new tab"
3. Copy that URL from the address bar

**pinterestUrl**: Just copy the URL of your Pinterest pin page

**affiliateUrl** (Amazon affiliate link):
1. Go to amazon.in and find the product
2. You'll see the SiteStripe bar at the top (grey bar)
3. Click "Text" → copy the short link like https://amzn.to/xxxxx?tag=yourtag-21

**productImage** (Amazon product image URL):
1. On the Amazon product page, right-click the main product image
2. "Open image in new tab" → copy that URL

**category options**: Skincare, Fashion, Makeup, Haircare, Accessories

---

## Deploy to Vercel (one time setup)

1. Create a free account at vercel.com
2. Install Vercel CLI:
   ```
   npm install -g vercel
   ```
3. Open terminal in the `glowpick` folder
4. Run:
   ```
   vercel
   ```
5. Follow the prompts — your site will be live in 60 seconds!

## Deploy updates (every time you add a new blog post)

After editing blogs.json, just run:
```
vercel --prod
```

That's it. Your site updates in ~30 seconds.

---

## Amazon Associate Rules (Important!)

- Your site MUST have this text visible: "As an Amazon Associate I earn from qualifying purchases." ✅ (already added to footer)
- Never fake reviews or ratings
- You earn 1%–9% commission depending on product category
- Payments are made monthly once you hit ₹2,500 minimum

---

## Categories & Commission Rates on Amazon.in

| Category | Commission |
|---|---|
| Fashion & Clothing | 9% |
| Beauty & Skincare | 9% |
| Shoes & Accessories | 9% |
| Health & Personal Care | 5% |
| Electronics | 2.5% |
