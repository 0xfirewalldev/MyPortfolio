# Irikefe M. Kesiena — Software Engineer & AppSec Specialist

> **"Engineering Resilience & Zero-Latency Scale."**  
> A high-performance, security-first portfolio showcasing modern full-stack application architecture and defensive vulnerability research.

[![Built with Astro](https://img.shields.io/badge/Astro-5.x-BC52EE.svg?style=flat-square&logo=astro&logoColor=white)](https://astro.build)
[![Tailwind CSS v4](https://img.shields.io/badge/Tailwind_CSS-v4-38B2AC.svg?style=flat-square&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![GSAP 3](https://img.shields.io/badge/Animations-GSAP_3-88CE02.svg?style=flat-square&logo=greensock&logoColor=white)](https://greensock.com)
[![TypeScript](https://img.shields.io/badge/Language-TypeScript-3178C6.svg?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)

---

## 🏛️ Architecture & Engineering Philosophy

This portfolio is built to reflect the dual discipline of its creator: **Full-Stack Software Architecture** and **Offensive Security Assessment**. Rather than relying on generic design templates, every component is intentionally crafted to demonstrate production-grade software standards:

- **Static-First Generation (SSG)**: Zero runtime JavaScript bloat by default using Astro’s component architecture.
- **Hardware-Accelerated Micro-Interactions**: GPU-composited animations via GSAP `quickTo` transforms to eliminate layout thrashing.
- **Defensive Design Patterns**: Zero-trust API schemas, sanitized client-side state, and strict accessibility compliance.
- **Terminal & System Telemetry Aesthetic**: An engineering-grade UI that merges minimal typography with interactive developer telemetry.

---

## 🛠️ Technology Stack & Toolchain

| Layer                | Technology                               | Purpose & Implementation                                                                  |
| -------------------- | ---------------------------------------- | ----------------------------------------------------------------------------------------- |
| **Framework**        | **Astro 5**                              | Server-first component compiler with zero-JS baseline and isolated routing.               |
| **Styling**          | **Tailwind CSS v4**                      | Next-generation engine utilizing modern CSS variables and lightning-fast compilation.     |
| **Animation Engine** | **GSAP 3 + ScrollTrigger**               | GPU-accelerated transforms (`scale`, `y`), timeline staging, and accessibility fallbacks. |
| **Type Safety**      | **TypeScript**                           | Strict compile-time validation across all component props and dataset schemas.            |
| **Iconography**      | **Astro Icon + Lucide + Simple Icons**   | Pure inline SVG compilation with zero client runtime overhead.                            |
| **Code Quality**     | **Prettier + Prettier Astro & Tailwind** | Automated code formatting and class ordering.                                             |

---

## 🔬 System Components & In-Depth Analysis

### 1. Hero Engine (`src/pages/_components/Hero.astro`)

- **Two-Column Responsive Grid**: Balances technical proposition typography against an interactive terminal interface.
- **Terminal Diagnostic Box (`HeroTerminal.astro`)**: Simulates an active command-line interface featuring simulated commands (`whoami`, `stack --list`, `audit ./app --owasp`) with a keyframe-animated blinking cursor.
- **Fluid Typography**: Responsive headline scaling (`text-4xl sm:text-6xl lg:text-7xl`) configured with leading bounds for visual punch without overflow.
- **Scroll Indicator**: Absolute-anchored discovery indicator featuring cubic-bezier keyframe physics and reduced-motion safety.

### 2. System Identity Bento Grid (`src/pages/_components/WhoAmI.astro`)

Structured into a mathematical 6-column modular bento grid (`md:grid-cols-6`):

- **Bio Card (`md:col-span-4`)**: Executive summary detailing Next.js, TypeScript, and AppSec philosophy, complete with active status tags and social gateway links.
- **Latest Activity (`md:col-span-2`)**: Dynamic telemetry feed with an active ping indicator tracking current research topics (`LEARNING`, `BUILDING`, `HARDENING`).
- **Interactive System Map (`SkillTree.astro` - `md:col-span-6`)**:
  - Dual-branch tree mapping **Build** (Construction) against **Break** (Deconstruction/Security).
  - Implements CSS subgrid (`md:grid-rows-subgrid`) to guarantee horizontal card alignment between complementary engineering and security disciplines.
  - Staggered GSAP ScrollTrigger batch animations with instant viewport hydration fallbacks.
- **Stats Metrics (`md:col-span-2`)**:
  - 2×2 metric matrix displaying critical indicators (0 Criticals in Prod, 0 Security Audits, 80% Projects Shipped, 2+ Years Experience).
  - Integrated **`SYS_INTEGRITY`** status footer with real-time operational status dot.
- **Security Arsenal & Toolchain (`md:col-span-4`)**:
  - Categorized weapons of choice: Offensive Security (`Burp Suite`, `Nmap`, `OWASP ZAP`, `SQLmap`), Runtime Stack (`Next.js`, `TypeScript`, `Supabase`, `Docker`), and Defense Standards (`OWASP Top 10`, `OAuth PKCE`, `IDOR Audit`).

### 3. macOS-Inspired Magnification Dock (`src/components/Dock.astro`)

- **Physics-Based Wave Falloff**: Icons dynamically magnify (`scale: 1.0` → `1.45`, `y: -8px`) using a cosine bell-curve algorithm based on cursor proximity (`RANGE: 110px`).
- **GPU Composited**: Built with `will-change: transform` and `transform-origin: 50% 100%` (`origin-bottom`) so icons scale upward from the dock shelf without triggering costly browser reflows.
- **Active Section Tracking**: High-performance `IntersectionObserver` observing `#works`, `#about`, and `#contact` to highlight the current scroll position.
- **Micro-Interactions**: Smooth anchor scrolling paired with a subtle physics-based bounce on click.

### 4. Works & Architecture Index (`/works`)

- **Curated Difficulty Hierarchy**:
  - **`Professional`**: Production-grade systems with complex integrations (e.g., _Sizer.io_ risk engine with TradingView API, _Vertex Canvas_ collaborative Kanban with HMAC-SHA256 session encryption).
  - **`Intermediate`**: Specialized tools and storefronts (e.g., _VulnTrack Lite_ Python/FastAPI CVE threat engine, _E&A Atelier_ luxury crochet storefront).
- **Work Type Segmentation**:
  - Distinct separation between **Core Architectures / Independent Labs** and **Commercial Client Deliverables**.
- **Zero-Dependency View Toggle**:
  - Client-side toggle between an expansive 2-column card grid and a compact single-column list view with full ARIA accessibility (`aria-pressed`).

### 5. Encrypted Dispatch Gateway (`/contact`)

- **Dedicated Route Architecture**: Follows the modular `layout/` and `pages/` pattern with its own layout shell.
- **Direct Dispatch**: Primary `mailto:` trigger with hover styling.
- **Interactive Clipboard Action**: Integrated Web Clipboard API with a 2-second visual feedback state (`Copied to Clipboard!`).
- **Scope of Engagement**: Dedicated breakdown for Full-Stack Architecture vs. AppSec & Pentesting scopes.
- **Response Telemetry**: Public SLA declaration (`< 24 Hours Guaranteed`), Timezone availability (`GMT+1 / Remote Global`), and verified security stance.
- **Terminal Status Footer**: Clean system-wide status declaration (`ALL SYSTEMS NOMINAL`) and copyright watermark.

### 6. Fault-Tolerant Error Handling (`src/pages/404.astro`)

- **System Alert Diagnostics**: Cyber-themed 404 screen styled with packet-drop alerts and a simulated terminal traceroute showing route failure.
- **Immediate Recovery Paths**: Actionable routes to return home, explore works, or contact the developer.

---

## 🔒 Defensive Security Patterns Implemented

1. **Safe Canonicalization**: Resilient URL construction handling undefined `Astro.site` configurations to prevent server crashes.
2. **Reverse Tabnabbing Protection**: Strict `rel="noopener noreferrer"` attributes applied to all external and third-party hyperlinks.
3. **Reduced Motion Compliance**: Comprehensive `@media (prefers-reduced-motion: reduce)` media queries across all GSAP timelines and CSS keyframes.
4. **Input Sanitization & Schema Safety**: Architected for strict Zod schema validation on forms and session-safe token storage across all featured projects.

---

## 📁 Project Directory Structure

```text
myportfolio/
├── public/
│   ├── favicon.ico
│   ├── favicon.svg
│   └── logo.svg
├── src/
│   ├── components/
│   │   ├── uiComp/
│   │   │   └── Navbar.astro            # Global top header navigation
│   │   ├── Dock.astro                  # Floating macOS magnification dock
│   │   ├── HeroTerminal.astro          # Interactive hero terminal simulation
│   │   ├── ScrollIndicator.astro       # Viewport physics scroll indicator
│   │   └── SkillTree.astro             # Interactive Build ↔ Break system map
│   ├── layout/
│   │   └── Layout.astro                # Primary document shell & SEO metadata
│   ├── pages/
│   │   ├── _components/
│   │   │   ├── Hero.astro              # Landing hero section
│   │   │   ├── WhoAmI.astro            # Modular identity bento grid
│   │   │   └── Contact.astro           # Contact section & clipboard gateway
│   │   ├── works/
│   │   │   ├── index.astro             # /works entrypoint
│   │   │   ├── layout/
│   │   │   │   └── WorkLayout.astro    # Dedicated works layout wrapper
│   │   │   └── pages/
│   │   │       └── Works.astro         # Curated works grid & list component
│   │   ├── 404.astro                   # Error handling & diagnostic gateway
│   │   └── index.astro                 # Homepage orchestrator
│   └── styles/
│       └── global.css                  # Tailwind CSS v4 entrypoint
├── astro.config.mjs                    # Astro configuration & integrations
├── package.json                        # Dependencies & build scripts
├── tsconfig.json                       # TypeScript compiler options
└── README.md                           # Technical portfolio documentation
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js**: `v22.23.4` or higher
- **Package Manager**: `npm`

### Installation

```bash
# Clone repository
git clone https://github.com/0xfirewalldev/myportfolio.git
cd myportfolio

# Install dependencies
npm install
```

### Local Development

```bash
# Start Astro development server
npm run dev

# Start development server in background mode (per workspace rules)
npx astro dev --background
```

The server will boot locally at `http://localhost:4321` (or `4322`).

### Production Build & Preview

```bash
# Validate types and generate production static assets
npm run build

# Preview production build locally
npm run preview
```

---

## 👤 Author

**Irikefe M. Kesiena**  
_Full-Stack Software Engineer & Cybersecurity Specialist_

- **GitHub**: [@0xfirewalldev](https://github.com/0xfirewalldev)
- **Twitter / X**: [@DevTech_Coder23](https://twitter.com/DevTech_Coder23)
- **Blog**: [zero-js-blog.vercel.app](https://zero-js-blog.vercel.app)
- **Email**: [kesienamichaels@gmail.com](mailto:kesienamichaels@gmail.com)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
