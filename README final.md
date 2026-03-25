# Dr. Asad Mehmood — Portfolio Website

> Personal portfolio website for Dr. Asad Mehmood, Specialist Prosthodontist & Implantologist, consulting in Mumbai.

---

## About This Website

This is a single-page portfolio website built with pure HTML, CSS, and JavaScript. No frameworks or dependencies required. Simply upload the `index.html` file and it works.

**Live Website:** [dr-asad-nine.vercel.app](https://dr-asad-nine.vercel.app)

---

## Pages & Sections

| Section | Description |
|---------|-------------|
| Hero | Name, tagline, credentials, profile photo placeholder, stats |
| About | Bio, clinical philosophy, four pillars |
| Specialist Services | 6 services with photo placeholders |
| Mumbai Consulting | Primary consultation focus |
| Experience | Professional journey timeline |
| Education | MDS · RGUHS, International License · Saudi Arabia, BDS · MUHS |
| Gulf Experience | Saudi license and Gulf credentials |
| Lifechanging Outcomes | Before & After slider with 4 cases |
| Testimonials | Patient voices section |
| Contact | Enquiry form with location details |

---

## How to Edit Content

All content is inside the single `index.html` file. Open it in any text editor or edit directly on GitHub.

### Change Your Name or Title
Search for `Dr. Asad Mehmood` and update as needed.

### Change Contact Details
Search for these placeholders and replace with your real information:
```
+91 80953 71362
drasadm.implants13@gmail.com
[Add your LinkedIn URL]
| Instagram | https://www.instagram.com/drasad_m.prostho/ |
```

### Change the Tagline
Search for `Crafting Smiles. Creating Confidence.` and replace with your preferred tagline.

---

## How to Add Photos

### Step 1: Upload Photos to GitHub
1. In this repository click **Add file** then **Upload files**
2. Create a folder called `images`
3. Upload your photos with simple names: `profile.jpg`, `smile-makeover.jpg` etc.
4. Click **Commit changes**

### Step 2: Replace Profile Photo (Hero Section)
Find this code:
```html
<div class="photo-placeholder">
```
Replace the entire placeholder div with:
```html
<img src="/images/profile.jpg" style="width:100%;height:100%;object-fit:cover;object-position:top;">
```

### Step 3: Replace Profile Photo (About Section)
Find this code:
```html
<div class="about-photo-empty">
```
Replace the entire div with:
```html
<img src="/images/profile.jpg" style="width:100%;height:100%;object-fit:cover;object-position:top;">
```

### Step 4: Replace Service Photos
Find this code for each service card:
```html
<div class="svc-photo-placeholder">
```
Replace the entire placeholder div with:
```html
<img src="/images/smile-makeover.jpg" style="width:100%;height:180px;object-fit:cover;margin-bottom:20px;">
```

Repeat for all 6 service cards with the relevant photo for each service.

### Step 5: Replace Before & After Photos
Find this code inside each slide:
```html
<div class="ba-photo-placeholder">
```
Replace with:
```html
<img src="/images/case1-before.jpg" style="width:100%;height:100%;object-fit:cover;">
```

### Recommended Photo Names

| Photo | Suggested Filename |
|-------|--------------------|
| Profile headshot | `profile.jpg` |
| Smile makeover | `smile-makeover.jpg` |
| Full mouth rehab | `full-mouth-rehab.jpg` |
| Dental implants | `dental-implants.jpg` |
| Cast partial denture | `partial-denture.jpg` |
| TMD treatment | `tmd.jpg` |
| Digital smile design | `digital-smile.jpg` |
| Case 1 before | `case1-before.jpg` |
| Case 1 after | `case1-after.jpg` |
| Case 2 before | `case2-before.jpg` |
| Case 2 after | `case2-after.jpg` |

---

## How to Add Testimonials

Find this section in `index.html`:
```html
<div class="t-text">Patient testimonial coming soon...</div>
<div class="t-name">Patient Name · Mumbai</div>
```
Replace with the real testimonial text and patient name or initials.

---

## How to Update Case Titles in the Slider

Find this line for each slide:
```html
<div class="slide-caption">Case 1 · Replace with your case title...</div>
```
Replace with your actual case title and brief description.

---

## How to Deploy on Vercel

1. Go to [vercel.com](https://vercel.com)
2. Sign up with your GitHub account
3. Click **Add New Project**
4. Select this repository
5. Click **Deploy**
6. Your website is live within 2 minutes

Every time you make a change to `index.html` or upload new photos on GitHub, Vercel automatically updates your live website within 1 to 2 minutes.

---

## File Structure

```
dr-asad-portfolio/
│
├── index.html          ← Main website file (all code in one file)
├── README.md           ← This guide
│
└── images/             ← Create this folder and add your photos here
    ├── profile.jpg
    ├── smile-makeover.jpg
    ├── dental-implants.jpg
    ├── full-mouth-rehab.jpg
    ├── partial-denture.jpg
    ├── tmd.jpg
    ├── digital-smile.jpg
    ├── case1-before.jpg
    ├── case1-after.jpg
    └── ...
```

---

## Color Palette

| Color | Hex Code | Used For |
|-------|----------|----------|
| Deep Brown | `#2c1a0e` | Headings, hero background |
| Brown | `#4a2c1a` | Dark backgrounds |
| Sienna | `#b5651d` | Accents, buttons, highlights |
| Amber | `#d4a843` | Secondary accents |
| Ivory | `#fdf6ed` | Page background |
| Warm Cream | `#fffaf3` | Card backgrounds |

---

## Placeholder Checklist

Before going live, complete the following:

- [ ] Add profile photograph (hero section)
- [ ] Add profile photograph (about section)
- [ ] Add your phone number
- [ ] Add your email address
- [ ] Add your LinkedIn profile URL
- [x] Instagram profile linked (drasad_m.prostho)
- [ ] Add service photos for all 6 services
- [ ] Add before & after case photos (with patient consent)
- [ ] Add real patient testimonials (with patient permission)
- [ ] Update case slide captions with real case titles

---

## Important Notes

- All patient photographs must be shared with **explicit patient consent**
- All testimonials must be provided with **patient permission**
- Do not add any credentials, qualifications, or clinical claims not verified by Dr. Mehmood
- The website is fully mobile responsive and works on all screen sizes

---

*Portfolio website for Dr. Asad Mehmood | Specialist Prosthodontist & Implantologist | Mumbai*

---

## How to Add a WhatsApp Direct Contact Button

A floating WhatsApp button allows patients to contact you instantly from any page. Here is exactly how to add it.

### Step 1: Add this code to your index.html

Open `index.html` on GitHub, click the pencil icon to edit, and paste the following code **just before** the closing `</body>` tag at the very bottom of the file:

```html
<!-- WHATSAPP FLOATING BUTTON -->
<a href="https://wa.me/918095371362?text=Hello%20Dr.%20Asad%2C%20I%20would%20like%20to%20book%20a%20consultation."
   class="whatsapp-float"
   target="_blank"
   rel="noopener noreferrer"
   aria-label="Chat on WhatsApp">
  <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
    <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/>
  </svg>
</a>

<style>
.whatsapp-float{
  position:fixed;
  bottom:28px;
  right:28px;
  width:58px;
  height:58px;
  background:#25d366;
  border-radius:50%;
  display:flex;
  align-items:center;
  justify-content:center;
  z-index:500;
  box-shadow:0 4px 20px rgba(37,211,102,0.4);
  transition:all 0.3s;
  text-decoration:none;
}
.whatsapp-float:hover{
  background:#20ba5a;
  transform:translateY(-4px) scale(1.08);
  box-shadow:0 8px 28px rgba(37,211,102,0.5);
}
.whatsapp-float svg{
  width:30px;
  height:30px;
  fill:#ffffff;
}
.whatsapp-float::before{
  content:'Chat with us';
  position:absolute;
  right:68px;
  background:#2c1a0e;
  color:#ffffff;
  font-family:'Nunito',sans-serif;
  font-size:11px;
  font-weight:600;
  letter-spacing:1px;
  padding:8px 14px;
  white-space:nowrap;
  opacity:0;
  transition:opacity 0.3s;
  pointer-events:none;
}
.whatsapp-float:hover::before{
  opacity:1;
}
</style>
```

### Step 2: Replace the phone number

Find this part in the code above:
```
https://wa.me/918095371362
```
Replace `918095371362` with your actual number. No spaces, no + sign, no dashes. Just country code followed by your number.

| Country | Format | Example |
|---------|--------|---------|
| India | `91` + number | `918095371362` |
| Saudi Arabia | `966` + number | `966501234567` |
| UAE | `971` + number | `971501234567` |

### Step 3: Customise the pre-filled message (optional)

In the link find this part:
```
?text=Hello%20Dr.%20Asad%2C%20I%20would%20like%20to%20book%20a%20consultation.
```
This message auto-fills when a patient taps the button. Change it to anything. Replace spaces with `%20` and commas with `%2C`.

### What the Button Does
- Floats fixed in the bottom right corner on every section
- Shows a tooltip `Chat with us` on hover
- Opens WhatsApp directly on mobile
- Opens WhatsApp Web on desktop
- Pre-fills a consultation message so patients do not need to type anything

