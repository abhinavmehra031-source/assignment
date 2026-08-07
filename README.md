# Accredian Enterprise Page (Partial Clone)

Recreation of the [Accredian Enterprise Website](https://enterprise.accredian.com/) built using Next.js (App Router), TypeScript, Tailwind CSS, Lucide Icons, and Framer Motion.

---

## 🌟 Live Demo & Preview
- **Local Dev Server:** `http://localhost:3000`
- **Lead Capture API Endpoint:** `http://localhost:3000/api/enquire`

---

## 🎯 Key Features & Implemented Scope

### 1. Complete Landing Page Sections
- 🧭 **Header Navigation:** Sticky glassmorphism header with logo branding ("accredian enterprise"), desktop section anchors, and mobile drawer menu.
- 🚀 **Hero Section:** High-converting headline ("Next-Gen Expertise For Your Enterprise"), value badges, CTA buttons ("Enquire Now" & "Explore Programs"), and interactive enterprise capability growth card stack.
- 📊 **Stats Counter Section:** "The Numbers Behind Our Success" displaying 10K+ Professionals Trained, 200+ Sessions Delivered, 5K+ Active Learners, and 50+ Enterprise Partners.
- 🤝 **Client Partners Section:** Corporate partner showcase featuring Reliance, HCL, IBM, CRIF, ADP, Bayer with capability trust badges.
- ⚡ **The Accredian Edge (7 Pillars):** Interactive grid highlighting Tailored Solutions, Expert Guidance, Innovative Framework, Advanced Technology, Diverse Offerings, Proven Impact, and Flexible Delivery.
- 🎯 **Domain Expertise (7 Tracks):** Program catalog for Gen-AI Mastery, Product & Innovation, Leadership Elevation, Tech & Data Insights, Operations Excellence, Digital Enterprise, and Fintech Innovation Lab.
- 📑 **Tailored Course Segmentation:** Interactive tabbed interface filtering by *Program Specific*, *Industry Specific*, *Topic Specific*, and *Level Specific*.
- 👥 **Who Should Join? (Strategic Enhancement):** Dedicated dark-navy section highlighting target audiences (Tech Professionals, Non-Tech Professionals, Emerging Professionals, Senior Executives).
- 🔄 **The CAT Framework:** Interactive 3-pillar learning framework (Concept, Application, Tools) with smooth tab switching.
- 🛠️ **Structured Delivery Approach:** 3-step operational workflow (Skill Gap Analysis → Customized Training Plan → Flexible Program Delivery).
- ❓ **FAQ Section:** Accordion tabs for *About the Course*, *About the Delivery*, and *Miscellaneous*.
- 💬 **Testimonials Carousel:** Interactive review carousel featuring enterprise L&D leaders from ADP, Bayer, CRIF, and HCL with star ratings and metrics.
- 📝 **Lead Capture System (Bonus Feature):**
  - Popup **Modal** triggered by "Enquire Now" CTAs across the page.
  - Embedded **Lead Capture Section** at the bottom of the page.
  - Asynchronous submission to Next.js API Route `/api/enquire` with form validation, loading states, and success feedback.
- ⚓ **Footer:** Corporate links, domain shortcuts, social links, contact information, and scroll-to-top button.

---

## 🛠️ Tech Stack

- **Framework:** Next.js 16 (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS v4 + Custom Glassmorphism & Keyframe Utilities
- **Icons:** Lucide React
- **Animations & Micro-interactions:** Framer Motion & CSS Keyframes
- **API Routes:** Next.js Route Handlers (`src/app/api/enquire/route.ts`)

---

## 🚀 Setup & Local Execution Instructions

### Prerequisites
- Node.js (v18.x or later)
- npm (v9.x or later)

### Steps

1. **Clone the Repository:**
   ```bash
   git clone <YOUR_GITHUB_REPOSITORY_URL>
   cd assignment
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Run Development Server:**
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) in your browser.

4. **Build for Production:**
   ```bash
   npm run build
   npm start
   ```

---

## 🤖 AI Usage Explanation (Mandatory Submission Requirement)

### Where AI Helped:
1. **Site Content Extraction & Structure Mapping:** Used AI browser tools to audit the original Accredian Enterprise website structure, extracting accurate section copy, FAQ items, and corporate client testimonials.
2. **Component Boilerplate Generation:** Accelerated initial React component creation and TypeScript interface declarations for domain tracks and course segmentation content.
3. **Design System & Tailwind Utility Drafting:** Assisted in mapping color codes (`#0066FF`, `#0B192C`), glassmorphism card blur rules, and marquee keyframe logic.

### What Was Modified & Improved Manually:
1. **Interactive Form State & Server API Validation:** Handled server-side validation rules in `/api/enquire/route.ts` (email regex checking, required field validation, and structured error responses).
2. **Modal & Preset Handling:** Enhanced user experience by allowing course cards to pass pre-selected program titles (e.g. "Gen-AI Mastery") directly into the Lead Capture modal.
3. **Accessibility & Responsive Polish:** Refined mobile menu drawer behavior, keyboard focus rings, touch targets, and dark/light contrast ratios for clean legibility across devices.
4. **Performance & Build Verification:** Resolved Next.js compilation trace issues and tuned component boundaries (`"use client"` vs static server rendering).

---

## 📈 Improvements With More Time

If allocated additional development time, the following enhancements would be added:
1. **Persistent Database Integration:** Replace the in-memory lead store with PostgreSQL + Prisma ORM or MongoDB Atlas for persistent storage.
2. **Automated Lead Email Notifications:** Integrate Resend or SendGrid to send instant confirmation emails to leads and notification alerts to the enterprise sales team.
3. **Protected Admin Dashboard (`/admin/leads`):** Build an internal management view to filter lead submissions by company size, program interest, and export to CSV.
4. **Interactive Enterprise ROI Calculator:** Add an interactive slider widget allowing corporate clients to estimate productivity gains and training cost savings based on team size.
5. **Comprehensive E2E Testing:** Implement Playwright / Cypress end-to-end tests for form submissions, modal toggles, and tab switches.

---

## 📦 Vercel Deployment Instructions

1. Push your code to GitHub:
   ```bash
   git add .
   git commit -m "Build Accredian Enterprise Clone with Lead Capture API"
   git push origin main
   ```
2. Go to [Vercel Dashboard](https://vercel.com/new).
3. Import your GitHub repository.
4. Keep framework preset as **Next.js** and click **Deploy**.
