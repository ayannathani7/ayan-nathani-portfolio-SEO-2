# Ayan Nathani | Personal Portfolio Website

![Ayan Nathani Portfolio Preview](assets/images/project-portfolio.svg)

> A modern, stylish, aesthetic, and fully responsive personal developer portfolio website built for **Ayan Nathani** (also searchable as *Nathani Ayan*) — Frontend Developer, Aspiring Full Stack Developer, AI Builder, Web Developer, and UI/UX Enthusiast. Currently a Diploma 3rd Semester student at GMIU, Bhavnagar, with verified internship experience at **Midnight Sphere**.

---

## 🌟 Highlights & Key Features

- 🌌 **Interactive 3D Particle Constellation (Canvas)**: Smooth HTML5 Canvas particle system simulating true 3D perspective depth, auto-rotation, and mouse inertia.
- 🎴 **Vanilla 3D Card Tilt Physics**: Perspective tilt on hover with dynamic holographic specular reflection/glare across hero card, service cards, skill cards, and project showcases.
- ⌨️ **Animated Hero Subtitle Typewriter**: Dynamic typing effect cycling through *Frontend Developer*, *AI Builder*, *Aspiring Full Stack Dev*, *UI/UX Enthusiast*, and *Web Developer*.
- 📩 **Serverless Web3Forms Client Message Studio (Direct to Gmail)**:
  - **Zero Database Required**: Direct serverless email dispatch via Web3Forms API (`https://api.web3forms.com/submit`) straight to `ayannathani7@gmail.com`.
  - **Client Topic Quick Pills**: Clients can choose *Frontend Dev*, *Responsive Web*, *AI Web App*, *UI/UX Design*, *Customization*, or *Internship* to auto-populate the subject.
  - **Live Character Counter & Field Validation**: Real-time validation with clean feedback alerts.
  - **Direct Gmail Web Composer Fallback**: Instant one-click fallback opening Gmail directly with prefilled parameters.
- 📜 **Midnight Sphere Internship Certificate Viewer**: Interactive modal displaying the verified internship certificate completed under CEO Arman Mahetar.
- 🌓 **Dark & Light Mode Toggle**: Seamless theme switching with persistent `localStorage` preference.
- 📱 **100% Mobile Responsive Layout**: Flawless experience from 320px smartphones to 4K desktop screens without any horizontal overflow.
- ⚡ **Zero Framework Dependencies**: Pure semantic HTML5, modern CSS3, and modular Vanilla JavaScript for ultra-fast load speed and Core Web Vitals.
- 🔍 **Advanced SEO & Technical Optimization**: Comprehensive Schema.org JSON-LD Person & WebSite markup, canonical tags, Google Search Console verification placeholder, OpenGraph, Twitter cards, `sitemap.xml`, and `robots.txt`.

---

## 🛠️ Tech Stack & Skills

- **Core Technologies**: Semantic HTML5, Modern CSS3 (Vanilla Design System), JavaScript (ES6+)
- **Tools & Ecosystem**: Figma, Git, GitHub, Antigravity IDE, VS Code, Browser DevTools
- **Specializations**: Responsive Web Design, UI/UX Design, AI Tools & Prompting, Frontend Architecture
- **Email Gateway**: [Web3Forms](https://web3forms.com/) (Serverless form-to-email)

---

## 📁 Project Directory Structure

```text
PORTFOLIO 2/
│
├── index.html                      # Main semantic HTML5 structure & SEO metadata
├── style.css                       # Complete CSS design system, 3D tilt, and responsive themes
├── script.js                       # 3D canvas constellation, 3D tilt, typewriter & Web3Forms logic
├── server.js                       # Lightweight Node.js localhost server (port 3000)
├── README.md                       # Complete documentation, customization & deployment guide
├── robots.txt                      # Crawler indexation directives for Google & search engines
├── sitemap.xml                     # Search engine XML sitemap
│
├── assets/
│   ├── images/
│   │   ├── project-portfolio.svg   # Personal Portfolio project illustration
│   │   ├── project-restaurant.svg  # Savory Bistro restaurant project illustration
│   │   ├── project-novamarket.svg  # NovaMarket e-commerce project illustration
│   │   ├── project-ai-studio.svg   # Nexus AI Studio web application illustration
│   │   ├── certificate-preview.svg # Midnight Sphere Internship certificate preview
│   │   └── avatar-illustration.svg # Modern developer avatar graphic
│   │
│   └── resume/
│       └── Ayan_Nathani_Resume.html # Printable / downloadable resume file
│
└── favicon/
    └── favicon.svg                 # Custom geometric <AN/> branding favicon
```

---

## 🚀 How to Run on Localhost

You have multiple zero-friction options to run the website locally:

### Option 1: Built-in Node.js Server (Recommended)
Run the included `server.js` file:
```bash
node server.js
```
Then visit **`http://localhost:3000`** in your browser.

### Option 2: Python HTTP Server
```bash
python -m http.server 3000
```
Then visit **`http://localhost:3000`**.

### Option 3: VS Code Live Server
1. Open the project folder in **VS Code**.
2. Right-click `index.html` and choose **"Open with Live Server"**.
3. It will launch at `http://127.0.0.1:5500`.

---

## ✉️ Web3Forms Setup Guide (Direct to Gmail)

This portfolio uses **[Web3Forms](https://web3forms.com/)** to deliver client enquiries directly to your Gmail inbox (**ayannathani7@gmail.com**) without requiring a server backend or custom database.

### Step 1: Obtain Your Web3Forms Access Key
1. Visit **[https://web3forms.com/](https://web3forms.com/)** in any browser.
2. In the "Enter your email" field, type your email address: **`ayannathani7@gmail.com`**.
3. Click the **"Create Access Key"** button.
4. Check your Gmail inbox for an email from Web3Forms containing your unique Access Key (e.g. `12345678-abcd-1234-abcd-1234567890ab`).

### Step 2: Configure the Access Key in `index.html`
1. Open [index.html](file:///c:/Users/Mahhmad%20nathani/OneDrive/Desktop/PORTFOLIO%202/index.html).
2. Locate the contact form around line ~1210:
   ```html
   <input type="hidden" name="access_key" value="YOUR_WEB3FORMS_ACCESS_KEY_HERE" id="web3forms-access-key" />
   ```
3. Replace **`YOUR_WEB3FORMS_ACCESS_KEY_HERE`** with your actual Access Key.
4. Save the file.

### Step 3: Verify Your Email & Test on Deployed Portfolio
1. Open your portfolio locally (`http://localhost:3000`) or on your deployed site (e.g., GitHub Pages).
2. Scroll to the **Contact & Message** section.
3. Fill in your name, a test email address, select an inquiry topic, type a short message, and click **"Send to Ayan's Gmail"**.
4. You will see a professional green success message: *"Enquiry Sent Successfully!"*.
5. Check your Gmail inbox at **`ayannathani7@gmail.com`**. You will receive an email with the subject:
   `New Portfolio Enquiry - Ayan Nathani: [Selected Topic] Project Inquiry`
   containing the visitor's name, reply-to email, and full message.

---

## 🗄️ Note on Persistent Database Storage (Supabase / Firebase)

> [!NOTE]
> **Web3Forms is a stateless form-to-email forwarding gateway.** It automatically validates submissions, checks for spam, and dispatches enquiries directly to your Gmail inbox. Web3Forms **does not** store your enquiries in your own personal database.

If you ever require long-term database storage (such as a private client admin dashboard or CRM) alongside email notifications, you can easily integrate a cloud database service:

### 1. Supabase (PostgreSQL)
1. Create a free project at [supabase.com](https://supabase.com/).
2. Create an `enquiries` table with columns: `id`, `name`, `email`, `subject`, `message`, `created_at`.
3. In `script.js`, after client validation, call the Supabase JavaScript client:
   ```javascript
   await supabase.from('enquiries').insert([{ name, email, subject, message }]);
   ```
4. Enable Row Level Security (RLS) with an `INSERT`-only policy for public visitors to protect your database.

### 2. Firebase Cloud Firestore
1. Create a Firebase project at [firebase.google.com](https://firebase.google.com/).
2. Initialize Firestore in your project using Firebase Web SDK.
3. Add submissions using `addDoc(collection(db, "enquiries"), { name, email, subject, message, timestamp: serverTimestamp() })`.
4. Configure Firestore security rules to allow `create` operations while disallowing public `read` or `delete`.

For most developer portfolios, Web3Forms email delivery directly to Gmail provides the fastest, most reliable, and maintenance-free setup.

---

## 🌐 Deployment Instructions

### 1. GitHub Pages (Free)
1. Push this repository to GitHub under your account (`github.com/ayannathani/portfolio`).
2. Go to **Settings** → **Pages**.
3. Under **Branch**, select `main` (or `master`) and folder `/ (root)`.
4. Click **Save**.
5. Your portfolio will be live at `https://ayannathani.github.io/`.

### 2. Vercel (Free & Fast)
1. Install Vercel CLI via `npm i -g vercel` or go to [vercel.com](https://vercel.com).
2. Import your GitHub repository.
3. Keep default settings (Static site) and click **Deploy**.
4. You will get a live production URL with automatic HTTPS and global edge CDN.

### 3. Netlify (Free Drag & Drop)
1. Log into [netlify.com](https://netlify.com).
2. Drag and drop this folder into the Netlify dashboard.
3. Your site is deployed in under 10 seconds.

---

## 🔍 Google Search Console & SEO Submission Checklist

To ensure search engines quickly crawl and rank your portfolio for **Ayan Nathani**, **Nathani Ayan**, and related developer keywords:

- [ ] **Custom Domain (Optional)**: If you purchase a domain like `ayannathani.dev` or `ayannathani.com`, update the canonical link and OpenGraph tags in `index.html`, and the URL in `sitemap.xml`.
- [ ] **Google Search Console**:
  1. Go to [search.google.com/search-console](https://search.google.com/search-console).
  2. Add your website property (e.g., `https://ayannathani.github.io/`).
  3. Choose **HTML Tag** verification. Copy the verification code and paste it into `index.html` replacing `GSC_VERIFICATION_PLACEHOLDER_AYAN_NATHANI`:
     ```html
     <meta name="google-site-verification" content="YOUR_COPIED_TOKEN" />
     ```
  4. Deploy the change and click **Verify** in Search Console.
- [ ] **Submit Sitemap**:
  1. In Google Search Console, navigate to **Sitemaps**.
  2. Enter `sitemap.xml` in the URL field and click **Submit**.
  3. Google will crawl your pages and index the structured data.
- [ ] **Rich Results Test**:
  - Test your URL at [search.google.com/test/rich-results](https://search.google.com/test/rich-results) to verify Schema.org Person & WebSite structured data.

---

## ✅ Final Quality & Testing Checklist

- [x] **Primary & Secondary SEO Keywords**: Accurately placed throughout `<title>`, `<meta description>`, `<h1>`, content paragraphs, and JSON-LD schema.
- [x] **3D Canvas Constellation**: High FPS, responsive resize, mouse inertia, auto-pause on background tab.
- [x] **3D Card Tilt**: Smooth physics with dynamic specular glare on all cards.
- [x] **Web3Forms Message Inbox**: Client topic selection, real-time validation, serverless Gmail dispatch, zero database dependency.
- [x] **Mobile Responsiveness**: Verified on mobile (320px–480px), tablet (768px), and desktop (1024px+).
- [x] **Theme Switcher**: Dark mode default with persistent light mode option in `localStorage`.
- [x] **Modals**: Full keyboard ESC and click-outside dismissal for certificate and project quick-views.
- [x] **Localhost Server**: Verified with `server.js` on port 3000.

---

© 2026 **Ayan Nathani**. Built with semantic HTML5, modern CSS3, and Vanilla JavaScript.
#   a y a n - n a t h a n i - p o r t f o l i o - S E O - 2  
 #   a y a n - n a t h a n i - p o r t f o l i o - S E O - 2  
 #   a y a n - n a t h a n i - p o r t f o l i o - S E O - 2  
 #   a y a n n a t h a n i - S E O - P O R T F O L I O - 2  
 