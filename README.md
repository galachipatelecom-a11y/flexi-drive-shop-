# Flexi Drive Shop

## ফোল্ডার
- `index.html`: পুরো সাইট (মোবাইল রেসপন্সিভ)
- `api/order.js`: অর্ডার টেলিগ্রামে পাঠায়
- `logos/`, `hero/`: ছবি। প্রথমে `.png` খোঁজে, না পেলে আগের সাইট, শেষে এই `.svg` ব্যাকআপ দেখায়
- `og-image.png`: ফেসবুকে লিংক শেয়ার করলে যে ছবি দেখায়
- `robots.txt`, `vercel.json`: সার্চ ও নিরাপত্তা সেটিংস

## GitHub থেকে চালু করা
1. ZIP খুলুন। ভেতরের সব ফাইল ও ফোল্ডার (`index.html` সহ) GitHub Repository-র একদম উপরের স্তরে আপলোড করুন।
2. vercel.com, Add New Project, ওই Repository ইমপোর্ট।
3. Settings, Environment Variables: `TELEGRAM_BOT_TOKEN` ও `TELEGRAM_CHAT_ID`।
4. Redeploy।

## নিজে বদলানোর জায়গা (`index.html`-এর `<script>`-এ `CFG`)
- `bkash`, `nagad`: পেমেন্ট নম্বর
- `messenger`, `whatsapp`, `telegram`: সাপোর্ট লিংক
- `fbPixel`, `ttPixel`: Meta ও TikTok Pixel ID (বসালে PageView, InitiateCheckout, Purchase/CompletePayment ইভেন্ট নিজে থেকে যায়)

## করণীয়
- `index.html`-এ `YOUR-DOMAIN` খুঁজে নিজের ডোমেইন বসান।
- আসল অফিশিয়াল লোগো থাকলে `logos/gp.png, bl.png, rb.png, at.png, tt.png, bkash.png, nagad.png` নামে দিন।
- নতুন অফারের দাম আনুমানিক, অ্যাপ দেখে যাচাই করুন।
- টোকেন কখনো কোডে লিখবেন না।
