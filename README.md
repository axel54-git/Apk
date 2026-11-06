# Markitify APK Download - Landing Page

A fast, responsive mobile web landing page for Markitify APK built with React, Vite, and Tailwind CSS.

---

## 🚀 Cloudflare Pages Deployment (ক্লাউডফেয়ার ডিপ্লয়মেন্ট গাইড)

### পদ্ধতি ১: GitHub কানেক্ট করে ডিপ্লয় (সবচেয়ে সহজ ও অটোমেটিক)

1. **[Cloudflare Dashboard](https://dash.cloudflare.com/)**-এ লগইন করুন।
2. বাঁপাশের মেনু থেকে **Workers & Pages** > **Create application** > **Pages** ট্যাবে যান।
3. **Connect to Git** সিলেক্ট করে আপনার GitHub অ্যাকাউন্ট (`axel54-git`) কানেক্ট করুন।
4. **`Apk`** রিপোজিটরিটি সিলেক্ট করে **Begin setup**-এ ক্লিক করুন।
5. **Build settings** এভাবে দিন:
   - **Framework preset:** `Vite`
   - **Build command:** `npm run build`
   - **Build output directory:** `dist`
   - **Root directory:** `/`
6. **Environment variables (Optional):**
   - Variable name: `NODE_VERSION`
   - Value: `20`
7. **Save and Deploy** বাটনে ক্লিক করুন। ২ মিনিটের মধ্যে আপনার সাইট লাইভ হয়ে যাবে!

---

### পদ্ধতি ২: Wrangler CLI দিয়ে ডিপ্লয় (কমান্ডের মাধ্যমে)

টার্মিনালে এই কমান্ডগুলো রান করুন:

```bash
# ১. ডিপেনডেন্সি ইনস্টল করুন
npm install

# ২. প্রোডাকশন বিল্ড তৈরি করুন
npm run build

# ৩. ক্লাউডফেয়ারে ডিপ্লয় করুন
npx wrangler pages deploy dist --project-name=markitify-apk
```

---

## 🛠️ লোকাল ডেভেলপমেন্ট

```bash
# ইনস্টল
npm install

# লোকাল ডেভ সার্ভার চালু
npm run dev

# টাইপ ও লিন্ট চেক
npm run lint
```
