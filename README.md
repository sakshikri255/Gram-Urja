# 🌾 GramUrja (GreenGrid AI)

<div align="center">

![GramUrja Logo](public/gramurja_logo.jpg)

### **AI-Powered Rural Sustainability & Clean Energy Intelligence Platform**
*Empowering Indian Gram Panchayats & Households with Waste-to-Energy, Solar Potential & Water Intelligence*

[![Vite](https://img.shields.io/badge/Vite-5.0-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)
[![React](https://img.shields.io/badge/React-18.2-61DAFB?logo=react&logoColor=black)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-3.4-38B2AC?logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Google Search Console Ready](https://img.shields.io/badge/SEO-Google%20Console%20Indexed-059669?logo=google)](https://gram-urja-alpha.vercel.app/sitemap.xml)

**🌐 Live Platform:** [https://gram-urja-alpha.vercel.app](https://gram-urja-alpha.vercel.app)

</div>

---

## 📑 Table of Contents

1. [Platform Overview](#-platform-overview)
2. [Key Capabilities & Modules](#-key-capabilities--modules)
3. [Monitored Bihar Gram Panchayats](#-monitored-bihar-gram-panchayats)
4. [Scientific Formulas & Indian Standards](#-scientific-formulas--indian-standards)
5. [Bilingual AI Architecture (Manu AI)](#-bilingual-ai-architecture-manu-ai)
6. [Tech Stack & Architecture](#-tech-stack--architecture)
7. [Repository Structure](#-repository-structure)
8. [Getting Started & Local Setup](#-getting-started--local-setup)
9. [SEO & Google Search Console Setup](#-seo--google-search-console-setup)
10. [Deployment on Vercel](#-deployment-on-vercel)
11. [Contributing & AI Development Guidelines](#-contributing--ai-development-guidelines)
12. [License & Acknowledgments](#-license--acknowledgments)

---

## 🌟 Platform Overview

**GramUrja (GreenGrid AI)** is an intelligent, physics-grounded rural sustainability platform engineered specifically for the Indian subcontinent. It bridges the gap between rural decentralized energy resources and decision-makers by converting raw village data into actionable clean energy roadmaps.

Designed for **Gram Panchayats, Block Development Officers (BDOs), and rural citizens**, GramUrja provides real-time modeling for:
- ☀️ **Rooftop & Ground-Mounted Solar Sizing** (under PM Surya Ghar Muft Bijli Yojana).
- 🐮 **Bio-methanation & SATAT Waste-to-Energy Recovery** (from cattle dung, agricultural crop residue, and kitchen waste).
- 💧 **Drinking Water Demands & Rainwater Harvesting** (benchmarked against Jal Jeevan Mission).
- ⚡ **Community Microgrids & Feeder Load Balancing** for 24x7 rural power reliability.
- 🎙️ **Bilingual Voice Interaction** via **Manu AI**, supporting Indian English (`en-IN`) and Hindi (`hi-IN`).

---

## 🚀 Key Capabilities & Modules

### 1. 🏛️ Gram Panchayat Command Centre (`/village`)
- **Multi-Village Switcher**: Immediate toggle between 5 Bihar model villages (*Motipur, Oiara, Amra, Barouni, Korha*).
- **Daily Feedstock Breakdown**: Granular organic waste statistics (`kg/day` of cattle dung, food waste, and crop biomass).
- **Grid Load Profiling**: Current vs. optimized peak load curves, baseline grid dependency, and annual savings projection.
- **Multidimensional Sustainability Score**: 0–100 weighted index evaluating solar readiness, organic waste circularity, water security, and grid autonomy.

### 2. ☀️ Solar Potential & Sizing Simulator (`/solar`)
- **Capacity Calculator**: Estimates feasible capacity in kW from roof surface area (sq ft) and monthly grid consumption.
- **Financial Payback & ROI**: Incorporates current MNRE capital costs (₹60,000/kW) and PM Surya Ghar subsidy tiers.
- **Carbon Abatement**: Accurately computes monthly CO₂ mitigation using CEA (Central Electricity Authority) 2023 grid factors (0.716 kg CO₂/kWh).

### 3. ♻️ Biogas & SATAT Waste-to-Energy Engine (`/waste`)
- **Multi-Stream Digester Modeling**: Computes biogas yield ($m^3/\text{day}$) from varied feedstock streams:
  - Cattle Dung: $0.04\ m^3/\text{kg}$
  - Food & Kitchen Waste: $0.08\ m^3/\text{kg}$
  - Agricultural Residue: $0.05\ m^3/\text{kg}$
- **Energy Conversion**: Calculates daily electrical generation ($1.8\ \text{kWh}/m^3$), thermal output ($5.5\ \text{kWh}/m^3$), and equivalent LPG cylinder offsets.
- **Bio-Slurry Fertilizer**: Computes organic fertilizer byproduct yield for zero-chemical farming.

### 4. 🏡 Household Energy & Appliance Audit (`/household`)
- **Appliance Wattage Tracker**: Interactive inventory (LED bulbs, BLDC ceiling fans, televisions, induction cooktops, submersible pumps).
- **Custom Appliance Builder**: Add custom loads with automated daily kWh calculation and monthly DISCOM cost projection.
- **BEE 5-Star Savings Advisor**: Smart tips to upgrade from inefficient legacy appliances to 5-star energy-efficient hardware.

### 5. 🔌 Community Microgrid & Feeder Hub (`/microgrid`)
- **Feeder Reliability Simulator**: Analyzes village feeder lines, battery storage (BESS), and solar microgrid clustering.
- **Peak Shaving Analysis**: Smooths out peak evening irrigation and domestic loads using stored solar and biogas power.

### 6. 💧 Water Demand & Rainwater Harvesting (`/water`)
- **JJM Benchmark**: Daily water demand calculation based on 55 Litres Per Capita per Day (LPCD).
- **RWH Potential**: Annual harvest yield calculation using local monsoon precipitation curves and runoff coefficients.
- **Solar Pump Sizing**: Sizing solar photovoltaic agricultural pumps (3 HP / 5 HP) to replace diesel pumps.

### 7. 🤖 Manu AI Conversational Assistant (`/ai`)
- **Bilingual Dialogue**: Fully responsive in English and Hindi.
- **Indian English Accent**: Synthesizes speech with native Indian cadence (`en-IN` profiles like *Microsoft Neerja* and *Google English India*).
- **Audio Voice Input**: Web Speech Recognition API with automatic noise handling and speech transcription.

---

## 📍 Monitored Bihar Gram Panchayats

The platform includes verified empirical data baselines for 5 Gram Panchayats in Bihar:

| Gram Panchayat | Households | Monthly Grid Load | Daily Organic Waste Feedstock | Feasible Solar | Solar Status |
|:---|:---:|:---:|:---|:---:|:---:|
| **Motipur** | 1,684 HH | 72,938 kWh | **1,684 kg/day** (Dung: 900kg, Food: 500kg, Agri: 284kg) | 150 kW | Planned |
| **Oiara** | 674 HH | 29,912 kWh | **674 kg/day** (Dung: 400kg, Food: 180kg, Agri: 94kg) | 100 kW | Feasible |
| **Amra** | 803 HH | 35,408 kWh | **803 kg/day** (Dung: 500kg, Food: 200kg, Agri: 103kg) | 125 kW | Feasible |
| **Barouni** | 300 HH | 13,980 kWh | **300 kg/day** (Dung: 180kg, Food: 80kg, Agri: 40kg) | 300 kW | **15 kW Active** |
| **Korha** | 170 HH | 7,842 kWh | **170 kg/day** (Dung: 100kg, Food: 45kg, Agri: 25kg) | 75 kW | Feasible |

---

## 📐 Scientific Formulas & Indian Standards

All mathematical models in [`src/calculations/engine.ts`](src/calculations/engine.ts) are strictly deterministic and benchmarked against official Indian government standards:

### 1. Solar Sizing & Carbon Abatement
$$\text{Feasible Capacity (kW)} = \min\left(\frac{\text{Roof Area (sq ft)}}{100},\ \frac{\text{Monthly Consumption (kWh)}}{120}\right)$$
$$\text{Monthly Generation (kWh)} = \text{Capacity (kW)} \times 4.5 \times 30$$
$$\text{Monthly Cost Savings (₹)} = \text{Monthly Generation (kWh)} \times \text{DISCOM Tariff (₹6.00/kWh)}$$
$$\text{CO}_2 \text{ Avoided (kg/month)} = \text{Monthly Generation (kWh)} \times 0.716\ \text{kg CO}_2\text{/kWh (CEA 2023)}$$

### 2. Biogas & SATAT Bio-methanation
$$\text{Biogas Yield } (m^3/\text{day}) = (\text{Dung kg} \times 0.04) + (\text{Food Waste kg} \times 0.08) + (\text{Crop Residue kg} \times 0.05)$$
$$\text{Daily Electrical Energy (kWh)} = \text{Biogas } (m^3/\text{day}) \times 1.8\ \text{kWh}/m^3$$
$$\text{Daily Thermal Energy (kWh)} = \text{Biogas } (m^3/\text{day}) \times 5.5\ \text{kWh}/m^3$$
$$\text{LPG Cylinder Equivalent (cylinders/mo)} = \frac{\text{Biogas } (m^3/\text{month}) \times 0.45}{14.2\ \text{kg}}$$

### 3. Jal Jeevan Mission Rural Water Demand
$$\text{Daily Village Water Demand (Litres)} = \text{Population} \times 55\ \text{LPCD (Jal Jeevan Mission Standard)}$$
$$\text{Rainwater Harvest Potential (L/yr)} = \text{Roof Area } (m^2) \times \text{Annual Rainfall (mm)} \times 0.85\ \text{(Runoff Coeff)}$$

---

## 🎙️ Bilingual AI Architecture (Manu AI)

Manu AI is GramUrja's voice-enabled rural intelligence assistant:
- **Speech Recognition**: Uses browser-native Web Speech API configured to `hi-IN` (Hindi) and `en-IN` (Indian English).
- **Speech Synthesis**: Priority voice matching for Indian English synthesizers (`Microsoft Neerja Online`, `Google हिन्दी`, `Microsoft Heera`, `Google English (India)`).
- **Deterministic Response Matching**: Deep intent categorization for subsidies (PM Surya Ghar, SATAT), solar payback, biogas yield, and water harvesting.

---

## 🛠️ Tech Stack & Architecture

| Layer | Technology | Purpose |
|:---|:---|:---|
| **Core Framework** | React 18.2 | Component-driven UI architecture |
| **Language** | TypeScript 5.2 | Strict typing, domain interfaces & contract safety |
| **Bundler & Dev Server**| Vite 5.1 | Sub-second HMR and optimized production bundling |
| **Styling** | Tailwind CSS 3.4 | Custom green-emerald dark theme + Glassmorphism |
| **Icons** | Lucide React | Clean, scalable vector interface icons |
| **Data Visualizations**| Recharts 2.12 | Responsive SVG charts (Radar, Bar, Area, Pie) |
| **Voice / Audio** | Web Speech API | Native in-browser speech synthesis & speech recognition |
| **Client Routing** | React Router DOM 6.22 | Client-side routing with role-based auth guards |
| **State Management** | React Context API | Distributed auth, language, and household load state |

---

## 📂 Repository Structure

```
Gram-Urja/
├── public/
│   ├── favicon.png             ← High-res platform icon
│   ├── favicon.jpg             ← Fallback favicon
│   ├── gramurja_logo.jpg       ← GramUrja official brand mark
│   ├── manu_ai_logo.jpg        ← Manu AI assistant avatar
│   ├── robots.txt              ← Search engine crawler instructions & sitemap link
│   ├── sitemap.xml             ← Standard XML Sitemap for Google Search Console
│   └── images/
│       └── landing_hero_bg.jpg ← Gemini AI cinematic rural clean-tech visual
├── src/
│   ├── ai/
│   │   └── chatEngine.ts       ← Manu AI deterministic response engine & intent matching
│   ├── calculations/
│   │   └── engine.ts           ← Mathematical formulas, MNRE constants & CEA factors
│   ├── components/
│   │   ├── AreaSelector.tsx    ← Gram Panchayat selector dropdown
│   │   ├── Layout.tsx          ← App shell, responsive navigation & floating Manu AI
│   │   └── ui.tsx              ← Reusable glassmorphic UI cards, badges & modals
│   ├── context/
│   │   ├── AuthContext.tsx     ← Role-based auth (Village Official, Citizen, Guest)
│   │   ├── HouseholdContext.tsx← Household appliance inventory & custom loads
│   │   └── LanguageContext.tsx ← Bilingual dictionary (English & Hindi translations)
│   ├── data/
│   │   ├── alerts.ts           ← Real-time anomaly detection alerts
│   │   ├── demoData.ts         ← 5 Bihar village profiles & feedstock metrics
│   │   ├── productData.ts      ← Solar panel, inverter, & biogas kit catalog
│   │   └── recommendations.ts  ← Prioritized action items ranked by ROI & carbon impact
│   ├── pages/
│   │   ├── AIAssistantPage.tsx ← Fullscreen Manu AI voice dialog page
│   │   ├── CommunityMicrogridPage.tsx ← Feeder & microgrid modeling
│   │   ├── HouseholdDashboard.tsx ← Household appliance & bill calculator
│   │   ├── LandingPage.tsx     ← Overview hub, 5 village login portals & live metrics
│   │   ├── LoginPage.tsx       ← Role selection & authentication portal
│   │   ├── RecommendationsPage.tsx ← Carbon & ROI ranked action plans
│   │   ├── SolarPage.tsx       ← Rooftop & land solar sizing simulator
│   │   ├── VillageDashboard.tsx← Gram Panchayat Command Centre
│   │   └── WastePage.tsx       ← SATAT bio-methanation & biogas simulator
│   ├── services/
│   │   └── energyService.ts    ← Analytical aggregation & village data adapters
│   ├── types/
│   │   └── index.ts            ← TypeScript type definitions & interfaces
│   ├── App.tsx                 ← Router configuration & route guards
│   ├── index.css               ← Tailwind CSS directives & custom glassmorphism styles
│   └── main.tsx                ← React DOM root mounting
├── index.html                  ← Entry HTML with SEO meta tags & Schema.org JSON-LD
├── vercel.json                 ← Vercel deployment single-page app rewrite configuration
├── tailwind.config.js          ← Tailwind theme configuration & custom color palette
├── tsconfig.json               ← TypeScript compiler settings
└── package.json                ← Dependencies & script definitions
```

---

## ⚡ Getting Started & Local Setup

### Prerequisites
- **Node.js** (v18.0.0 or higher recommended)
- **npm** (v9.0.0 or higher) or **yarn** / **pnpm**

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sakshikri255/Gram-Urja.git
   cd Gram-Urja
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the local development server:**
   ```bash
   npm run dev
   ```
   Open [http://localhost:5173](http://localhost:5173) in your browser.

4. **Build for production:**
   ```bash
   npm run build
   ```

5. **Preview the production bundle locally:**
   ```bash
   npm run preview
   ```

---

## 🔍 SEO & Google Search Console Setup

GramUrja is fully optimized for discovery and indexing on **Google Search Console**:

### 1. XML Sitemap (`/sitemap.xml`)
An XML sitemap conforming to Sitemaps Protocol 0.9 is available in [`public/sitemap.xml`](public/sitemap.xml) and served at `/sitemap.xml`. It indexes all routes:
- `/` (Home & Role Portal)
- `/overview` (Impact Overview Hub)
- `/village` (Gram Panchayat Command Centre)
- `/household` (Household Energy Tracker)
- `/solar` (Solar Potential Simulator)
- `/waste` (Biogas & SATAT Simulator)
- `/microgrid` (Community Microgrid Hub)
- `/recommendations` (Prioritized Action Plans)
- `/ai` (Manu AI Assistant)

### 2. Robots.txt (`/robots.txt`)
Located in [`public/robots.txt`](public/robots.txt), it allows all search engine bots to crawl the application and directs them to the sitemap:
```txt
User-agent: *
Allow: /
Sitemap: https://gram-urja-alpha.vercel.app/sitemap.xml
```

### 3. Structured Data (JSON-LD)
`index.html` embeds standard Schema.org structured metadata:
- **`@type: WebApplication`**: Documents application category (`UtilitiesApplication`), operating system, and feature lists.
- **`@type: Organization`**: Brand metadata with official logo and repository links.

### 4. How to Index on Google Search Console
1. Visit [Google Search Console](https://search.google.com/search-console).
2. Add your property using **URL prefix**: `https://gram-urja-alpha.vercel.app` (or your custom domain).
3. Verify ownership via **HTML tag** (already embedded in `index.html`).
4. Navigate to **Sitemaps** in the left sidebar.
5. Enter `sitemap.xml` and click **Submit**.
6. Google will automatically crawl and index all platform routes.

---

## 🚀 Deployment on Vercel

The application includes a [`vercel.json`](vercel.json) configuration for clean Single Page Application (SPA) routing:

```json
{
  "rewrites": [
    {
      "source": "/(.*)",
      "destination": "/index.html"
    }
  ]
}
```

### Deploy Steps
1. Push your changes to GitHub.
2. Import the repository in [Vercel](https://vercel.com).
3. Framework Preset: **Vite**.
4. Build Command: `npm run build`.
5. Output Directory: `dist`.
6. Click **Deploy**.

---

## 🤖 Contributing & AI Development Guidelines

For AI coding agents and contributors:
- Consult [AGENTS.md](AGENTS.md) for architectural guardrails and mathematical calculation invariants.
- Consult [IBM_BOB_Usage.md](IBM_BOB_Usage.md) for IBM BOB AI optimization standards.
- Always verify TypeScript compilation (`npm run build`) before submitting changes.
- Ensure all newly added UI strings are localized in `src/context/LanguageContext.tsx` for both English and Hindi.

---

## 📄 License & Acknowledgments

- **License**: MIT License.
- **Data Standards**: Benchmarked against standards by **MNRE (Ministry of New and Renewable Energy)**, **CEA (Central Electricity Authority)**, and **Jal Jeevan Mission (Ministry of Jal Shakti)**.
- **Built for**: Rural Clean Energy Transition & Smart Gram Panchayat Intelligence.

<div align="center">
  <sub>GramUrja © 2026 · Transforming Indian Villages with Sustainable Clean Intelligence</sub>
</div>
