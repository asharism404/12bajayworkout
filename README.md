# 12bajay workout

Static single-file app (index.html). No build step.

## Deploy (free, about 1 minute)
- Netlify: https://app.netlify.com/drop and drag this folder in.
- Vercel: `npx vercel --prod` inside the folder.
- GitHub Pages: push to a repo, then Settings > Pages > deploy from main.

## Payments
Edit `CFG.pay` at the top of the script in index.html with your Razorpay/UPI payment links.
Pro status is stored in the browser, so verify payments server-side before relying on it.
