# Dr. Asad Mehmood — Portfolio Website

> Personal portfolio website for Dr. Asad Mehmood, Specialist Prosthodontist & Implantologist, consulting in Mumbai.

**Live Website:** [dr-asad-new-website.vercel.app](https://dr-asad-new-website.vercel.app)

---

## About This Website

Single-page portfolio website built with pure HTML, CSS and JavaScript. All images are embedded directly in the file — no external image folder required. Simply upload `index.html` and it works immediately.

---

## Sections

| Section | Description |
|---------|-------------|
| Hero | Name, tagline, credentials, profile photo, stats |
| Marquee | Scrolling strip of specialties |
| About | Bio, clinical philosophy quote, four pillars |
| Specialist Services | 6 services with photos |
| Mumbai Consulting | Primary consultation focus |
| Experience | Professional journey timeline |
| Education | MDS RGUHS, Saudi License, BDS MUHS |
| Gulf Experience | Saudi license and credentials |
| Lifechanging Outcomes | Before & After slider with 3 cases |
| Patient Reviews | 3 real reviews + Google Review button |
| Contact | Form with phone, email, LinkedIn, Instagram |

---

## Contact Details Currently in Website

| Field | Details |
|-------|---------|
| Phone | +91 80953 71362 |
| Email | drasadm.implants13@gmail.com |
| LinkedIn | linkedin.com/in/dr-asad-mehmood-a6a713b7 |
| Instagram | @drasad_m.prostho |
| WhatsApp | +91 80953 71362 |
| Google Reviews | share.google/snlQBsWAkOvD4UFmS |

---

## How to Update Content

All content is inside the single `index.html` file. Edit it directly on GitHub using the pencil icon.

### Update the Tagline
Search for `Crafting Smiles. Creating Confidence.` and replace.

### Update Contact Details
Search for the current value and replace:
- Phone: `80953 71362`
- Email: `drasadm.implants13@gmail.com`
- WhatsApp number: `wa.me/918095371362`

### Update Google Review Link
Search for `share.google/snlQBsWAkOvD4UFmS` and replace with your updated link.

### Add or Update Testimonials
Search for `testimonial-card` and update the review text and patient name inside each card.

---

## How to Add or Replace Photos

Since all images are embedded as base64 in the HTML, the easiest way to replace a photo is to ask Claude to embed the new photo directly by uploading it in the chat.

If you want to do it manually:

### Step 1: Convert your photo to base64
1. Go to **base64.guru/converter/encode/image**
2. Upload your photo
3. Copy the base64 string

### Step 2: Find the image in index.html
Search for the alt text of the image you want to replace:

| Photo | Search for |
|-------|-----------|
| Hero profile photo | `alt="Dr. Asad Mehmood" style="border` |
| About profile photo | `alt="Dr. Asad Mehmood"/>` |
| Smile Makeovers | `alt="Esthetic Smile Makeovers"` |
| Full Mouth Rehab | `alt="Full Mouth Rehabilitation"` |
| Dental Implants | `alt="Dental Implants"` |
| Partial Denture | `alt="Cast Partial Dentures"` |
| TMD | `alt="Temporomandibular Disorders"` |
| Digital Smile | `alt="Digital Smile Design"` |

### Step 3: Replace the src value
Find `src="data:image/jpeg;base64,XXXX"` and replace the base64 string with your new one.

---

## How to Add a New Case to the Slider

Copy this block and paste inside the `slider-track` div:

```html
<div class="slide">
  <div class="ba-container">
    <div class="ba-panel">
      <img src="YOUR_BEFORE_BASE64_HERE" alt="Before"/>
      <div class="ba-label before-label">Before</div>
    </div>
    <div class="ba-divider">
      <div class="ba-divider-line"></div>
      <div class="ba-divider-icon">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
          <path d="M8 3L3 8l5 5M16 3l5 5-5 5"/>
        </svg>
      </div>
    </div>
    <div class="ba-panel">
      <img src="YOUR_AFTER_BASE64_HERE" alt="After"/>
      <div class="ba-label after-label">After</div>
    </div>
  </div>
  <div class="slide-caption">Transformation</div>
</div>
```

Then update the `total` variable in the JavaScript from `3` to `4`.

---

## How to Add a New Testimonial

Find the `testimonial-grid` div and add a new card:

```html
<div class="testimonial-card ripple-container reveal delay-1">
  <div class="t-quote">"</div>
  <div class="t-stars">&#9733;&#9733;&#9733;&#9733;&#9733;</div>
  <div class="t-text">Patient review text goes here.</div>
  <div class="t-name">Patient Name · Mumbai</div>
</div>
```

---

## How to Deploy on Vercel

1. Go to [vercel.com](https://vercel.com) and sign in with GitHub
2. Click **Add New Project**
3. Select your repository
4. Set **Framework Preset** to **Other**
5. Leave Build Command and Output Directory blank
6. Click **Deploy**

Every time you commit a change to GitHub, Vercel automatically redeploys within 1 to 2 minutes.

---

## How to Force Redeploy on Vercel

1. Go to vercel.com and open your project
2. Click **Deployments**
3. Click the three dots **...** next to the latest deployment
4. Click **Redeploy**
5. Wait 2 minutes and open your live URL

---

## WhatsApp Button

The floating WhatsApp button is live at the bottom right corner. To change the number search for `wa.me/918095371362` and replace with your new number (country code + number, no spaces or symbols).

---

## Color Palette

| Color | Hex | Used For |
|-------|-----|----------|
| Deep Brown | `#2c1a0e` | Hero background, dark sections |
| Brown | `#4a2c1a` | Dark text, hover states |
| Sienna | `#b5651d` | Primary accent, buttons |
| Amber | `#d4843a` | Secondary accent, gold elements |
| Ivory | `#fdf6ed` | Page background |
| Warm Cream | `#fffaf3` | Card backgrounds |

---

## File Structure

```
Dr-Asad-Portfolio-website/
│
├── index.html      ← Complete website, all images embedded
└── README.md       ← This guide
```

No images folder needed. Everything is self-contained in `index.html`.

---

## Checklist

- [x] Profile photograph embedded
- [x] Phone — +91 80953 71362
- [x] Email — drasadm.implants13@gmail.com
- [x] LinkedIn linked
- [x] Instagram — @drasad_m.prostho
- [x] WhatsApp button active
- [x] Google Review button linked
- [x] 3 real patient testimonials — Farhana Wali, Shrishti, Pratik
- [x] Before & after case photos — 3 cases
- [x] All 6 service photos embedded
- [ ] Additional case photos (add when available with patient consent)
- [ ] Additional testimonials (add as they come in)

---

## Important Notes

- All patient photographs are shared with explicit patient consent
- All testimonials are real and provided with patient permission
- Do not add credentials or clinical claims not verified by Dr. Mehmood
- The website is fully mobile responsive

---

*Dr. Asad Mehmood | Specialist Prosthodontist & Implantologist | Mumbai*
