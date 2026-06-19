# Shyraa Enterprises Hub

> A modern, responsive corporate website for Shyraa Enterprises — a Bengaluru-based supplier of scaffolding systems, aluminium ladders, and cable management solutions with all-India supply capability.

---

## Project Overview

**Shyraa Enterprises Hub** is a production-ready single-page application built to showcase the company's infrastructure products and services. The website serves as the digital storefront for Shyraa Enterprises, enabling potential customers to explore product offerings, learn about the company, and submit enquiries directly through an integrated contact form.

### Business Details
- **Company:** Shyraa Enterprises
- **Location:** Bengaluru Rural, Karnataka – 562162
- **Contact Person:** Harish
- **Phone:** 9880690929, 7619171474
- **Email:** Shyraaenterprises@gmail.com
- **Coverage:** All-India Supply | 24/7 Availability

---

## Features

### 1. Responsive Design
- Fully responsive layout optimized for mobile, tablet, and desktop screens
- Fluid typography and spacing using Tailwind CSS container system
- Touch-friendly navigation with minimum 44px tap targets
- Safe area support for notched devices (iPhone, Android)

### 2. Product Showcase
- Clean card-based product display for Scaffolding Systems and Aluminium Ladders
- Animated product cards with hover effects and shadow transitions
- Detailed item lists within each product category

### 3. Contact Section
- Enquiry form with client-side and server-side validation
- Fields: Name (required), Phone (optional), Email (optional), Address (optional), Message (required)
- Form data persisted to Supabase database
- Real-time validation with toast notifications
- Helper text for optional fields to improve UX

### 4. Mobile-Friendly Navigation
- Fixed top navbar with backdrop blur
- Hamburger menu for mobile devices with smooth open/close
- Active state indicators and touch-optimized buttons
- Click-to-call "Call Now" button for immediate contact

### 5. SEO Optimization
- Semantic HTML structure with proper heading hierarchy
- Meta tags for description, author, and robots
- Open Graph (OG) tags for social sharing
- Twitter Card support
- Canonical URL configuration
- Theme color and favicon for mobile web app experience
- Alt text on all images

### 6. Fast Loading Performance
- Vite-based build system for optimized bundling
- Code-splitting and tree-shaking
- Minimal third-party dependencies
- Font preloading via Google Fonts CDN
- CSS custom properties for consistent theming

### 7. Animations & Interactions
- Scroll-triggered entrance animations using Framer Motion
- Animated hero section with staggered reveals
- Smooth scroll behavior across anchor links
- Interactive hover states on cards and buttons
- Loading states for form submission

### 8. Security & Accessibility
- Client-side input validation (length checks, regex patterns)
- XSS prevention through proper React escaping
- Accessible form labels and focus rings
- Semantic landmarks for screen readers

---

## Technologies Used

### Core Framework & Language
| Technology | Purpose |
|------------|---------|
| **React 18** | UI library for building component-based interfaces |
| **TypeScript** | Type-safe JavaScript with static type checking |
| **Vite 5** | Next-generation frontend build tool and dev server |

### Styling & UI
| Technology | Purpose |
|------------|---------|
| **Tailwind CSS v3** | Utility-first CSS framework for rapid styling |
| **shadcn/ui** | Accessible, reusable UI component primitives |
| **Radix UI** | Unstyled, accessible UI primitives (dialogs, dropdowns, etc.) |
| **Tailwind CSS Animate** | Built-in animation utilities for Tailwind |

### Backend & Database
| Technology | Purpose |
|------------|---------|
| **Supabase** | Backend-as-a-Service (PostgreSQL database, REST API) |
| **PostgreSQL** | Relational database for storing contact enquiries |
| **PostgREST** | Auto-generated REST API from database schema |

### State Management & Data Fetching
| Technology | Purpose |
|------------|---------|
| **TanStack Query (React Query)** | Server-state management and data fetching |

### Routing & Navigation
| Technology | Purpose |
|------------|---------|
| **React Router DOM v6** | Client-side routing for single-page application |

### Animation
| Technology | Purpose |
|------------|---------|
| **Framer Motion** | Declarative animations and gestures for React |

### Forms & Validation
| Technology | Purpose |
|------------|---------|
| **React Hook Form** | Performant, flexible form handling |
| **Zod** | TypeScript-first schema validation |
| **@hookform/resolvers** | Zod resolver integration for React Hook Form |

### Icons & UI Enhancements
| Technology | Purpose |
|------------|---------|
| **Lucide React** | Beautiful, consistent SVG icon library |
| **Sonner** | Toast notification system |
| **Embla Carousel** | Lightweight carousel/slider component |
| **Recharts** | Composable charting library |
| **Date-fns** | Modern date utility library |

### Development & Tooling
| Technology | Purpose |
|------------|---------|
| **ESLint 9** | Static code analysis and linting |
| **TypeScript ESLint** | TypeScript-specific linting rules |
| **PostCSS** | CSS processing and transformations |
| **Autoprefixer** | Automatic vendor prefixing for CSS |
| **Vitest** | Unit testing framework |
| **@testing-library/react** | React component testing utilities |
| **jsdom** | Browser environment simulation for tests |

### Hosting & Deployment
| Technology | Purpose |
|------------|---------|
| **Lovable** | Visual development and deployment platform |
| **Lovable Cloud** | Managed backend with Supabase integration |

---

## Project Structure

```
shyraa-enterprises-hub/
├── public/                          # Static assets served at root
│   ├── favicon.ico                  # Site favicon
│   ├── placeholder.svg              # Placeholder image
│   └── robots.txt                   # Search engine crawl instructions
│
├── src/                             # Main application source code
│   ├── assets/                      # Project assets (images, logos)
│   │   └── logo.png                 # Company logo image
│   │
│   ├── components/                  # React components
│   │   ├── ui/                      # shadcn/ui primitive components
│   │   │   ├── accordion.tsx
│   │   │   ├── alert-dialog.tsx
│   │   │   ├── alert.tsx
│   │   │   ├── aspect-ratio.tsx
│   │   │   ├── avatar.tsx
│   │   │   ├── badge.tsx
│   │   │   ├── breadcrumb.tsx
│   │   │   ├── button.tsx
│   │   │   ├── calendar.tsx
│   │   │   ├── card.tsx
│   │   │   ├── carousel.tsx
│   │   │   ├── chart.tsx
│   │   │   ├── checkbox.tsx
│   │   │   ├── collapsible.tsx
│   │   │   ├── command.tsx
│   │   │   ├── context-menu.tsx
│   │   │   ├── dialog.tsx
│   │   │   ├── drawer.tsx
│   │   │   ├── dropdown-menu.tsx
│   │   │   ├── form.tsx
│   │   │   ├── hover-card.tsx
│   │   │   ├── input-otp.tsx
│   │   │   ├── input.tsx
│   │   │   ├── label.tsx
│   │   │   ├── menubar.tsx
│   │   │   ├── navigation-menu.tsx
│   │   │   ├── pagination.tsx
│   │   │   ├── popover.tsx
│   │   │   ├── progress.tsx
│   │   │   ├── radio-group.tsx
│   │   │   ├── resizable.tsx
│   │   │   ├── scroll-area.tsx
│   │   │   ├── select.tsx
│   │   │   ├── separator.tsx
│   │   │   ├── sheet.tsx
│   │   │   ├── sidebar.tsx
│   │   │   ├── skeleton.tsx
│   │   │   ├── slider.tsx
│   │   │   ├── switch.tsx
│   │   │   ├── table.tsx
│   │   │   ├── tabs.tsx
│   │   │   ├── textarea.tsx
│   │   │   ├── toast.tsx
│   │   │   ├── toaster.tsx
│   │   │   ├── toggle-group.tsx
│   │   │   ├── toggle.tsx
│   │   │   └── tooltip.tsx
│   │   │
│   │   ├── AboutSection.tsx         # About / Why Choose Us section
│   │   ├── ContactSection.tsx       # Contact form & info section
│   │   ├── Footer.tsx               # Site footer with links
│   │   ├── HeroSection.tsx          # Hero / landing banner
│   │   ├── NavLink.tsx              # Navigation link component
│   │   ├── Navbar.tsx               # Top navigation bar
│   │   └── ProductsSection.tsx      # Product showcase section
│   │
│   ├── hooks/                       # Custom React hooks
│   │   ├── use-mobile.tsx           # Mobile breakpoint detection
│   │   └── use-toast.ts             # Toast notification hook
│   │
│   ├── integrations/                # Third-party service integrations
│   │   └── supabase/
│   │       ├── client.ts              # Supabase client initialization
│   │       └── types.ts               # Auto-generated Supabase types
│   │
│   ├── lib/                         # Utility libraries
│   │   └── utils.ts                   # cn() helper and common utilities
│   │
│   ├── pages/                       # Page-level route components
│   │   ├── Index.tsx                  # Home page (single-page app)
│   │   └── NotFound.tsx               # 404 error page
│   │
│   ├── test/                        # Test configuration and examples
│   │   ├── example.test.ts            # Sample test file
│   │   └── setup.ts                   # Test environment setup
│   │
│   ├── App.css                      # Global app-specific styles
│   ├── App.tsx                      # Root app component with router
│   ├── index.css                    # Global CSS with Tailwind directives
│   ├── main.tsx                     # Application entry point
│   └── vite-env.d.ts                # Vite environment type declarations
│
├── supabase/                        # Supabase configuration
│   ├── config.toml                    # Supabase CLI configuration
│   └── migrations/                    # Database migration files
│       ├── 20260407142722_e1a5a0fd-1271-4f18-9394-303eb7190874.sql
│       └── 20260407143446_7630e7ab-4e3e-4bd0-a92f-7cf2ab4d8ff1.sql
│
├── .env                             # Environment variables (gitignored)
├── .env.example                     # Environment variable template
├── components.json                  # shadcn/ui configuration
├── eslint.config.js                 # ESLint configuration
├── index.html                       # HTML entry point with SEO meta tags
├── package.json                     # Project dependencies and scripts
├── postcss.config.js                # PostCSS configuration
├── README.md                        # Project documentation
├── tailwind.config.ts               # Tailwind CSS theme configuration
├── tsconfig.json                    # TypeScript root configuration
├── tsconfig.app.json              # TypeScript app-specific config
├── tsconfig.node.json             # TypeScript Vite/Node config
├── vite.config.ts                 # Vite build and dev configuration
└── vitest.config.ts               # Vitest test configuration
```

### Directory Explanations

| Directory | Description |
|-----------|-------------|
| `public/` | Static files copied directly to build output. Includes favicon, robots.txt, and placeholder assets. |
| `src/assets/` | Imported assets processed by Vite (logo images, etc.). |
| `src/components/ui/` | shadcn/ui component primitives — reusable, accessible, unstyled base components. |
| `src/components/` | Business-specific React components organized by page section. |
| `src/hooks/` | Custom React hooks for shared logic (mobile detection, toasts). |
| `src/integrations/supabase/` | Supabase client setup and auto-generated TypeScript types from database schema. |
| `src/lib/` | Shared utility functions (className merging with `cn()`). |
| `src/pages/` | Route-level components. Single-page app uses `Index.tsx` as the main page. |
| `src/test/` | Test files and Vitest configuration. |
| `supabase/migrations/` | SQL migration files for database schema evolution. |

---

## Frontend Details

### Architecture
The frontend follows a **single-page application (SPA)** architecture with a section-based landing page design. All content is rendered on one page with smooth anchor scrolling between sections.

### Page Structure (`src/pages/Index.tsx`)
```
Navbar (Fixed top navigation)
├── HeroSection (Full-screen landing banner)
├── ProductsSection (Product categories in cards)
├── AboutSection (Company features and value props)
├── ContactSection (Form + contact info)
└── Footer (Links and copyright)
```

### Component Breakdown

#### `Navbar.tsx`
- Fixed position header with `bg-primary/95` and backdrop blur
- Company logo + name on the left
- Desktop navigation links with hover transitions
- Mobile hamburger menu with slide-down panel
- Prominent "Call Now" CTA button linking to `tel:`

#### `HeroSection.tsx`
- Full-viewport height hero with gradient background (`bg-hero`)
- Animated text reveals using Framer Motion (`initial` → `animate`)
- Scroll-down arrow indicator with infinite bounce animation
- Two CTAs: "Explore Products" and "Get A Quote"
- Trust badges: "All-India Supply" and "24/7 Available"

#### `ProductsSection.tsx`
- Two-column grid showcasing product categories
- Card-based layout with icon, title, description, and item list
- Hover effects: background color shift and shadow elevation
- Staggered scroll-triggered animations

#### `AboutSection.tsx`
- Dark-themed section (`bg-section-dark`) with gradient
- Four feature cards in a responsive grid (1 → 2 → 4 columns)
- Icon + title + description for each feature
- Features: All-India Supply, 24/7 Availability, Quality Assured, Trusted Partner

#### `ContactSection.tsx`
- Two-column layout: Contact Info (left) + Enquiry Form (right)
- **Contact Info Card:**
  - Contact person: Harish
  - Clickable phone numbers
  - Clickable email link
  - Full business address
  - Operating hours (24/7)
  - All-India supply badge
- **Enquiry Form:**
  - Name (required, max 100 chars)
  - Phone Number (optional, 7–15 digits)
  - Email Address (optional, validated format)
  - Address (optional, max 500 chars)
  - Message (required, max 1000 chars)
  - Submit button with loading state
  - Form validation with toast error/success messages
  - Data submitted to Supabase `contact_enquiries` table

#### `Footer.tsx`
- Logo + company name + tagline
- Quick navigation links
- Copyright notice with dynamic year

### Styling Architecture

#### Tailwind CSS Configuration (`tailwind.config.ts`)
- **Custom Font Families:**
  - `font-sans`: Inter (body text)
  - `font-display`: Oswald (headings)
- **Color System:** HSL CSS variables for theming
  - `primary`: Navy blue (#1e3a5f area)
  - `secondary`: Orange (#e67e22 area)
  - `background`, `foreground`, `card`, `muted`, `destructive`
  - `orange-glow`, `navy-light` custom tokens
- **Border Radius:** Centralized via `--radius` CSS variable
- **Custom Animations:**
  - `fade-up`: Entry from below with opacity
  - `slide-in-right`: Entry from right with opacity
  - `accordion-down/up`: Content expand/collapse
- **Shadows:** `shadow-card`, `shadow-card-hover` with custom colors

#### Global CSS (`src/index.css`)
- Google Fonts import (Inter + Oswald)
- Tailwind directives (`@tailwind base/components/utilities`)
- CSS custom properties in `:root` for light mode
- `.dark` class for dark mode overrides
- Global styles: smooth scroll, text-size-adjust, overflow-x hidden
- Touch target minimums for mobile (`min-height: 44px`)
- Safe area padding utility for notched devices
- Custom utility classes: `.text-gradient`, `.bg-hero`, `.bg-section-dark`, `.shadow-card`, `.shadow-card-hover`

### Routing
- **Library:** React Router DOM v6
- **Router Type:** `BrowserRouter` (history API)
- **Routes:**
  - `/` → `Index` (home page with all sections)
  - `*` → `NotFound` (404 catch-all)
- **Navigation:** Anchor links (`#home`, `#products`, `#about`, `#contact`) for in-page scrolling

### Responsiveness Strategy
| Breakpoint | Behavior |
|------------|----------|
| `< 640px` (sm) | Single column, mobile nav, reduced font sizes, full-width buttons |
| `640px – 768px` (sm/md) | Two-column grids begin, larger tap targets |
| `768px+` (md) | Desktop nav visible, multi-column layouts |
| `1024px+` (lg) | Full spacing, max-width containers |
| `1280px+` (xl) | Optimal reading widths |
| `1536px+` (2xl) | Max container width `1400px` |

### Form Validation Logic
```
Name:    Required, trim, max 100 chars
Phone:   Optional, if filled: regex ^[0-9]{7,15}$
Email:   Optional, if filled: regex ^[^\s@]+@[^\s@]+\.[^\s@]+$
Address: Optional, max 500 chars
Message: Required, trim, max 1000 chars
```

---

## Backend Details

### Supabase Integration

#### Database Schema
**Table:** `public.contact_enquiries`

| Column | Type | Constraints | Description |
|--------|------|-------------|-------------|
| `id` | `uuid` | PRIMARY KEY, auto-generated | Unique enquiry identifier |
| `created_at` | `timestamp with time zone` | DEFAULT now() | Submission timestamp |
| `name` | `text` | NOT NULL | Customer name |
| `phone` | `text` | NULLABLE | Customer phone number |
| `email` | `text` | NULLABLE | Customer email address |
| `address` | `text` | NULLABLE | Customer address |
| `message` | `text` | NOT NULL | Enquiry message content |

#### Row Level Security (RLS)
- **INSERT Policy:** Anonymous users can submit enquiries (required for public contact form)
- **SELECT Policy:** Authenticated users with appropriate roles can read submissions
- **No anonymous sign-ups** enabled
- Data access controlled via RLS policies and GRANT statements

#### Database Client
```typescript
// src/integrations/supabase/client.ts
import { createClient } from '@supabase/supabase-js';
import type { Database } from './types';

export const supabase = createClient<Database>(
  import.meta.env.VITE_SUPABASE_URL,
  import.meta.env.VITE_SUPABASE_PUBLISHABLE_KEY,
  {
    auth: {
      storage: localStorage,
      persistSession: true,
      autoRefreshToken: true,
    }
  }
);
```

#### Type Generation
- Auto-generated TypeScript types in `src/integrations/supabase/types.ts`
- Strongly typed database queries with full IntelliSense support
- Table types: `Row`, `Insert`, `Update`, `Relationships`

### API Flow (Contact Form Submission)
```
User fills form → Client validation → Supabase insert →
Success: Show toast + Reset form → Error: Show error toast
```

### Security Measures
- Environment variables for Supabase credentials (never hardcoded)
- Client-side validation before API call
- Input sanitization (trim, length limits, regex patterns)
- XSS protection through React's built-in escaping
- SQL injection prevention via Supabase's parameterized queries
- No sensitive credentials exposed in client bundle (anon key only)

### Authentication
- Supabase Auth is configured but the public contact form does not require authentication
- Google OAuth can be configured for admin/role-based access
- Session persistence via localStorage

### Edge Functions
- Not currently deployed (migrations handle schema changes directly)
- Server-side rate limiting and honeypot spam protection can be added via Edge Functions if needed

---

## Installation Guide

### Prerequisites
- **Node.js** v18+ (recommended: v20+)
- **npm** or **bun** package manager
- **Git** for cloning

### Step 1: Clone the Repository
```bash
git clone <YOUR_GIT_URL>
cd <YOUR_PROJECT_NAME>
```

### Step 2: Install Dependencies
```bash
npm install
```
Or if using Bun:
```bash
bun install
```

### Step 3: Configure Environment Variables
Create a `.env` file in the project root:
```env
VITE_SUPABASE_URL=https://your-project.supabase.co
VITE_SUPABASE_PUBLISHABLE_KEY=your-anon-key
VITE_SUPABASE_PROJECT_ID=your-project-id
```

> **Note:** The publishable key is safe for the client. Never expose the service role key.

### Step 4: Start the Development Server
```bash
npm run dev
```

The dev server will start at `http://localhost:8080` (or the next available port).

### Step 5: Build for Production
```bash
npm run build
```

Output will be generated in the `dist/` directory.

### Step 6: Run Tests
```bash
npm run test
```

For watch mode:
```bash
npm run test:watch
```

---

## Deployment Guide

### Deploy via Lovable (Recommended)
1. Open your project in [Lovable](https://lovable.dev)
2. Click **Share → Publish** in the top-right corner
3. Your site will be live at a `.lovable.app` subdomain
4. For a custom domain: **Project Settings → Domains → Connect Domain**

### Frontend vs Backend Deployment
- **Frontend changes** (UI, styling, client code): Require clicking "Update" in the Publish dialog
- **Backend changes** (database migrations, edge functions): Deploy automatically

### Self-Hosting (Optional)
1. Build the project: `npm run build`
2. Serve the `dist/` folder from any static hosting (Netlify, Vercel, Cloudflare Pages, AWS S3)
3. Configure environment variables on your hosting platform
4. Update Supabase CORS settings to allow your domain

### SPA Routing
- Lovable hosting has built-in SPA fallback
- Deep links and page refreshes work automatically with React Router `BrowserRouter`
- No `_redirects` or `.htaccess` files needed

---

## Environment Variables

| Variable | Required | Description |
|----------|----------|-------------|
| `VITE_SUPABASE_URL` | Yes | Supabase project URL (e.g., `https://xxx.supabase.co`) |
| `VITE_SUPABASE_PUBLISHABLE_KEY` | Yes | Supabase anonymous/public API key |
| `VITE_SUPABASE_PROJECT_ID` | Yes | Supabase project ID string |

> All environment variables must be prefixed with `VITE_` to be exposed to the Vite client bundle.

---

## Complete Dependency List

### Production Dependencies (`dependencies`)
```
@hookform/resolvers          ^3.10.0
@radix-ui/react-accordion    ^1.2.11
@radix-ui/react-alert-dialog ^1.1.14
@radix-ui/react-aspect-ratio ^1.1.7
@radix-ui/react-avatar       ^1.1.10
@radix-ui/react-checkbox     ^1.3.2
@radix-ui/react-collapsible  ^1.1.11
@radix-ui/react-context-menu ^2.2.15
@radix-ui/react-dialog       ^1.1.14
@radix-ui/react-dropdown-menu ^2.1.15
@radix-ui/react-hover-card   ^1.1.14
@radix-ui/react-label        ^2.1.7
@radix-ui/react-menubar      ^1.1.15
@radix-ui/react-navigation-menu ^1.2.13
@radix-ui/react-popover      ^1.1.14
@radix-ui/react-progress     ^1.1.7
@radix-ui/react-radio-group  ^1.3.7
@radix-ui/react-scroll-area  ^1.2.9
@radix-ui/react-select       ^2.2.5
@radix-ui/react-separator   ^1.1.7
@radix-ui/react-slider      ^1.3.5
@radix-ui/react-slot        ^1.2.3
@radix-ui/react-switch      ^1.2.5
@radix-ui/react-tabs        ^1.1.12
@radix-ui/react-toast       ^1.2.14
@radix-ui/react-toggle       ^1.1.9
@radix-ui/react-toggle-group ^1.1.10
@radix-ui/react-tooltip      ^1.2.7
@supabase/supabase-js        ^2.102.1
@tanstack/react-query        ^5.83.0
class-variance-authority     ^0.7.1
clsx                         ^2.1.1
cmdk                         ^1.1.1
date-fns                     ^3.6.0
embla-carousel-react         ^8.6.0
framer-motion                ^12.34.0
input-otp                    ^1.4.2
lucide-react                 ^0.462.0
next-themes                  ^0.3.0
react                        ^18.3.1
react-day-picker             ^8.10.1
react-dom                    ^18.3.1
react-hook-form              ^7.61.1
react-resizable-panels       ^2.1.9
react-router-dom             ^6.30.1
recharts                     ^2.15.4
sonner                       ^1.7.4
tailwind-merge               ^2.6.0
tailwindcss-animate          ^1.0.7
vaul                         ^0.9.9
zod                          ^3.25.76
```

### Development Dependencies (`devDependencies`)
```
@eslint/js                   ^9.32.0
@tailwindcss/typography      ^0.5.16
@testing-library/jest-dom     ^6.6.0
@testing-library/react        ^16.0.0
@types/node                  ^22.16.5
@types/react                 ^18.3.23
@types/react-dom             ^18.3.7
@vitejs/plugin-react-swc     ^3.11.0
autoprefixer                 ^10.4.21
eslint                       ^9.32.0
eslint-plugin-react-hooks    ^5.2.0
eslint-plugin-react-refresh  ^0.4.20
globals                      ^15.15.0
jsdom                        ^20.0.3
lovable-tagger               ^1.1.13
postcss                      ^8.5.6
tailwindcss                  ^3.4.17
typescript                   ^5.8.3
typescript-eslint            ^8.38.0
vite                         ^5.4.19
vitest                       ^3.2.4
```

---

## Tech Stack Summary

| Layer | Technology |
|-------|------------|
| **Framework** | React 18 + TypeScript 5 |
| **Build Tool** | Vite 5 |
| **Styling** | Tailwind CSS 3 + shadcn/ui |
| **UI Primitives** | Radix UI |
| **Animation** | Framer Motion |
| **Icons** | Lucide React |
| **State Management** | TanStack Query |
| **Routing** | React Router DOM 6 |
| **Forms** | React Hook Form + Zod |
| **Backend** | Supabase (PostgreSQL + PostgREST) |
| **Testing** | Vitest + @testing-library/react + jsdom |
| **Linting** | ESLint 9 + TypeScript ESLint |
| **Fonts** | Inter (body), Oswald (headings) via Google Fonts |
| **Hosting** | Lovable / Lovable Cloud |

---

## Package Information

| Field | Value |
|-------|-------|
| **Name** | vite_react_shadcn_ts |
| **Version** | 0.0.0 |
| **Type** | ES Module (`"type": "module"`) |
| **Private** | Yes |
| **License** | Unspecified (add if needed) |

### Available Scripts
| Script | Command | Purpose |
|--------|---------|---------|
| `dev` | `vite` | Start development server with HMR |
| `build` | `vite build` | Production build |
| `build:dev` | `vite build --mode development` | Development mode build |
| `lint` | `eslint .` | Lint all source files |
| `preview` | `vite preview` | Preview production build locally |
| `test` | `vitest run` | Run unit tests once |
| `test:watch` | `vitest` | Run unit tests in watch mode |

---

## Screenshots

> Add screenshots of the deployed website below. Replace the placeholder paths with actual image URLs.

### Desktop View
| Section | Preview |
|---------|---------|
| **Hero Section** | ![Hero Section](./screenshots/desktop-hero.png) |
| **Products Section** | ![Products Section](./screenshots/desktop-products.png) |
| **About Section** | ![About Section](./screenshots/desktop-about.png) |
| **Contact Section** | ![Contact Section](./screenshots/desktop-contact.png) |
| **Footer** | ![Footer](./screenshots/desktop-footer.png) |

### Mobile View
| Section | Preview |
|---------|---------|
| **Mobile Hero** | ![Mobile Hero](./screenshots/mobile-hero.png) |
| **Mobile Navigation** | ![Mobile Nav](./screenshots/mobile-nav.png) |
| **Mobile Contact Form** | ![Mobile Form](./screenshots/mobile-form.png) |

---

## License

This project is proprietary to Shyraa Enterprises. All rights reserved.

---

## Author

**Shylaja M**

---

## Contact

For questions about this project, please reach out:

- **Business:** Shyraa Enterprises
- **Location:** 3rd Floor, No.C-25, Vajarahalli Road, Near Nelamangala, Bengaluru Rural, Karnataka – 562162
- **Phone:** 9880690929, 7619171474
- **Email:** Shyraaenterprises@gmail.com

---

<p align="center">
  Built with <a href="https://lovable.dev">Lovable</a> | React | TypeScript | Tailwind CSS | Supabase
</p>
