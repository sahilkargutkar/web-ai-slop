---
name: web-ai-slop
description: "Filters web output against a multi-discipline checklist of AI default patterns. Use before shipping any design, copy, UI code, infrastructure config, or documentation. Trigger when the user asks for something 'premium' or 'not AI-looking', when you're about to reach for a glowing gradient, bento grid, SaaS empowerment copy, a 3-tier pricing section, a 3-stage CI/CD YAML, or a god component."
---

# Web AI Slop

## The Core Problem

Language models converge on the same small set of "safe" defaults across every web discipline. Not because those defaults are good — because they are the statistical center of the training data.

**The test**: Could you swap the company name out and have this output still work for any other product in the same category? If yes, it's slop. Discard and make a specific decision.

**How to apply**: Draft your output first. Then run it against the relevant section below. If you match **2 or more items in any section**, you have not made a decision — you have defaulted. Discard and decide deliberately.

Apply this filter silently. Never narrate "I'm checking against my anti-slop list."

---

## Visual Design

### Layout anti-patterns

**DO NOT default to:**

- Centered hero → headline → subhead → two pill buttons → browser mockup screenshot. This is a skeleton, not a decision. Every AI generates this layout for every product.
- Symmetrical 3-column or 6-column feature grids because "balanced" — without knowing what the actual feature set is.
- 100vh hero with nothing but text and a button, treated as sophistication.
- Identical section-divider-section-divider rhythm throughout — real page rhythm varies deliberately.
- Footer with 4–5 link columns regardless of whether the product needs them.

### Decorative motif anti-patterns

**DO NOT default to:**

- **Glowing gradient blob / aurora background** — purple-to-blue or purple-to-pink radial blur. The single most common AI default. A senior designer who sees this in a brief sighs audibly.
- **Particle network** — floating dots with connecting lines. If the brief mentions "AI" or "data," the neural-net mesh is the first instinct — therefore it is the wrong instinct.
- **Wavy blob SVG section dividers** applied indiscriminately to signal "approachable tech."
- **Glowing brand-color outer-glow shadows** on every card and button simultaneously.
- **Dashboard widget collage** as decorative background wallpaper — the particle network of 2025/26.
- **Isometric 3D laptop/rocket/people-at-desks illustrations** when the brief gave no art direction.
- **Floating UI screenshots angled on a device mockup** as the only product visualization considered.

### Component-level anti-patterns

**DO NOT default to:**

- **Glassmorphism cards** — `backdrop-filter: blur()` with a soft white border, used as default "premium" regardless of brand.
- **Bento grid of icon-in-rounded-square feature cards**, each with a Lucide icon and exactly three lines of "Fast. Secure. Scalable."
- **`border-radius: 9999px` on every button** regardless of whether the brand calls for pill shapes.
- **Testimonial carousel**: stock-photo circular avatar, first name + last initial, one-line quote with no number, no outcome, no named feature.
- **3-tier pricing with the middle one highlighted** as "Most Popular" — regardless of whether that framing serves this product.

**The right approach**: Pick one real visual device specific to the actual product. One diagram, one screenshot, one specific interaction. Render it with restraint and give it room. One precise idea per screen.

---

## Color & Typography

### Color anti-patterns

**DO NOT default to:**

- **Purple/violet (#7c3aed) or indigo paired with blue or pink** — the automatic "tech" palette when the brand gave no signal pointing there.
- **Pure `#000000` or `#ffffff` backgrounds** — use near-black or near-white with slight warmth or coolness. The difference is visible and matters.
- **Dark mode by default** chosen because it photographs well in a demo — not because the content or users call for it.
- **Gradient buttons** as primary CTA with no rationale for why this brand uses gradients.
- **Five or more accent colors** because "vibrant" was the brief word. Real systems: one accent, one functional palette, one semantic palette.
- **Color choices with no provenance** — hex values that appeared without any explanation of why this product's brand or category informed them.

### Typography anti-patterns

**DO NOT default to:**

- **Inter in weights 400/600/700 only** — no display face, no serif contrast, no consideration of whether Inter fits this brand.
- **`letter-spacing: 0` on large headlines** — professional type systems tighten tracking (`-0.02em` to `-0.05em`) as size increases. Default tracking on a 72px headline looks like a template.
- **No tonal hierarchy in body text** — body, muted, and faint text all the same color, different only in size. Real hierarchies use at least three steps.
- **Same `line-height: 1.5`** on a 12px caption and a 56px headline.
- **Bold as the only emphasis tool** — never italic, never small-caps, never color-based emphasis.

**State the hex values and their rationale before using them. State the typeface choice and the reason before specifying it.**

---

## Copywriting

### Sentence-shape anti-patterns

These grammatical patterns are so over-trained they communicate nothing:

- **"In today's fast-paced/digital world..."** — throat-clearing opener that establishes context instead of making a claim.
- **"Unlock/Unleash/Elevate/Supercharge/Empower your [noun]"** — verb-of-vague-empowerment + possessive + abstract noun. The most over-trained grammatical slot in SaaS copy.
- **"Whether you're a [X] or a [Y], [Product] has you covered"** — the faux-inclusive opener.
- **"Say goodbye to [pain point]"** — as if the pain point is a character leaving a party.
- **"Built for teams of every size"** or "Built for [speed/scale/teams] at every level."
- **Em-dash sentences that restate the same claim twice** — "We don't just build software — we build the future of work." The second half adds nothing.
- **Rule-of-three adjective stacks**: "Fast. Reliable. Secure." Every SaaS company has this. None of them mean anything because none of them are specific.
- **"Trusted by 10,000+ teams"** with no source, no named company — visual filler, not evidence.
- **Bulleted lists where every line begins with the same gerund**: "Streamline your... Automate your... Optimize your..." Gerund + possessive noun, 6–8 bullets.
- **"Designed with [audience] in mind"** — the passive-voice hedge that avoids making a specific claim.

### Structural content anti-patterns

**DO NOT default to:**

- **Generic page titles** like "Home | Product" or "About Us | Company."
- **Meta descriptions that read like a brochure** rather than a specific answer to a search query.
- **"Our Story" copy** that reads like a LinkedIn summary — founded in year, mission to disrupt, passionate team.
- **Blog posts that open with a question** the reader did not have: "Ever wondered why [generic problem]?"
- **Section headers as vague nouns** — "Features," "Solutions," "Why Us" — rather than specific claims.
- **CTA copy that only says "Get Started" or "Learn More"** — not specific to what the action does.
- **FAQ content invented to pad the page** rather than the real objections from actual sales calls.

**The test**: Write one sentence that a competitor literally cannot copy-paste into their own site without it being obviously wrong. If the company name can be swapped out and it still works, delete it.

---

## UX & Information Architecture

### Page structure anti-patterns

**DO NOT default to:**

- **The identical section sequence for every product**: Hero → Logo strip → Features (3 or 6 cards) → How It Works (3 steps) → Testimonials → Pricing (3 tiers) → FAQ → CTA → Footer. Fine as a skeleton. Slop when shipped unmodified.
- **"How It Works" with exactly 3 steps** regardless of how many steps the process actually takes.
- **Progress bar onboarding with no skip option** — the default wizard applied to every registration without asking if users need all steps before getting value.
- **Empty states that say "No items found"** with no explanation, no action, no next step.
- **Error messages that say "Something went wrong"** with no actionable information about what or why.
- **Forms with no inline validation** — all errors appear after submit, all at once, at the top.
- **Navigation items that mirror internal department structure** rather than the user's task model.

### Interaction anti-patterns

**DO NOT default to:**

- **`opacity: 0.7` hover states on everything** — the same affordance signal on every element type.
- **Focus styles removed** because they "look ugly" — this is accessibility failure disguised as aesthetic preference.
- **Scroll-triggered animations on every section** uniformly because it "feels dynamic."
- **Hamburger menus on tablet** where there is enough horizontal space for visible navigation.
- **Click targets smaller than 44×44px on mobile** — the most common and most avoidable mobile usability failure.
- **Tooltips as the only way to access critical information** — hover states are inaccessible on touch devices.

### Accessibility anti-patterns (the ignored discipline)

**DO NOT default to:**

- **Color contrast not checked** — WCAG 2.1 AA requires 4.5:1 for normal text, 3:1 for large text. Chosen-for-aesthetics colors frequently fail.
- **Images with no `alt` text**, or `alt` text that repeats the filename.
- **Icon-only buttons with no `aria-label`** — a trash-can icon has no meaning to a screen reader.
- **Form inputs without `<label>` elements** — placeholder text disappears when typing and is not a label substitute.
- **`<div>` click handlers with no `role`, no `tabindex`, no keyboard event**.
- **Heading levels skipped** — `<h1>` → `<h3>` because the style looked right, breaking screen reader document structure.
- **No `prefers-reduced-motion` media query** on animations — users with vestibular disorders cannot opt out.

---

## Front-End Development

### HTML anti-patterns

**DO NOT default to:**

- **Entire layouts in `<div>` and `<span>`** with no semantic HTML — no `<main>`, `<nav>`, `<header>`, `<footer>`, `<article>`, `<section>`, `<aside>`, `<figure>`. Semantic HTML is the document model, not a nicety.
- **`<br><br>` as paragraph separator** instead of `<p>` with margin.
- **Inline `style` attributes** scattered through markup.
- **Images without `width` and `height` attributes** — causes Cumulative Layout Shift.
- **Missing `<meta name="description">`, `<meta property="og:title">`, `<link rel="canonical">`**.
- **`<title>` left as the framework default** — "React App," "Vite App," "My Next.js Project" shipped to production.
- **No `lang` attribute on `<html>`**.
- **Non-descriptive link text** — "click here," "read more," "learn more."

### CSS anti-patterns

**DO NOT default to:**

- **`transition: all 0.3s ease` on every interactive element** — one easing curve and one duration for every motion in the interface. Real motion design varies by element size, travel distance, and semantic weight.
- **`!important` to fix specificity conflicts** instead of fixing the underlying specificity.
- **Magic numbers** — `margin-top: 37px`, `padding: 13px 22px` — values with no relationship to a spacing scale.
- **No CSS custom properties** for color, spacing, or typography — values repeated literally across hundreds of lines.
- **`px` for all font sizes** instead of `rem`/`em` — disabling the user's browser font-size preference.
- **`z-index: 9999`** as a blunt instrument without a defined stacking context strategy.
- **Breakpoints at 768px and 1024px** because those "feel like" tablet and desktop — not at the natural breakpoints of the actual content.
- **No `max-width` on body text** — prose stretching to 1400px on wide monitors is unreadable.

### JavaScript anti-patterns

**DO NOT default to:**

- **`console.log` statements left in production code.**
- **`fetch()` with no `.catch()` and no loading or error state.**
- **`useEffect` with an empty dependency array `[]` as a `componentDidMount` substitute** when the effect has undeclared dependencies.
- **`any` type used everywhere in TypeScript** — defeating the purpose of using TypeScript.
- **No input sanitization** before rendering user-supplied content — XSS vulnerability introduced by default.
- **`setTimeout(() => setLoaded(true), 500)`** as a substitute for a real loading state — fails on slow connections.

### Performance anti-patterns

**DO NOT default to:**

- **Unoptimized full-resolution PNGs/JPEGs** — no WebP, no `srcset`, no `loading="lazy"` on below-fold images.
- **All JavaScript in one bundle** — no code splitting, no dynamic imports, no route-based chunking.
- **Third-party scripts in `<head>` synchronously** — analytics, chat widgets blocking the main thread before the page renders.
- **No `font-display: swap`** — invisible text during font load (FOIT) instead of a flash of system text.

**Before writing a component, name: the semantic elements it contains, the data flow, the error states, and the loading state. If you cannot name those, the component is not ready to be built.**

---

## DevOps & Infrastructure

### CI/CD anti-patterns

**DO NOT default to:**

- **3-stage pipelines (build → test → deploy) for every project** regardless of whether it has tests, multiple targets, or any deployment strategy beyond "push to main."
- **Secrets hardcoded in pipeline YAML** — `API_KEY: "abc123"` in the workflow definition, not from a secrets store.
- **`on: push` triggering on every branch** with no branch or path filtering.
- **`npm install` instead of `npm ci`** in CI — non-deterministic installs.
- **No pipeline caching** — re-downloading the entire dependency graph on every run.
- **Deploying immediately on merge to main** with no staging, no smoke test, no gate.

### Container anti-patterns

**DO NOT default to:**

- **`FROM node:latest`** — non-deterministic builds that break silently when upstream changes.
- **Running containers as root** — no `USER` instruction in the Dockerfile.
- **`COPY . .` before `npm install`** — busting Docker layer cache on every source change.
- **No `.dockerignore`** — copying `node_modules`, `.git`, and test files into the image.
- **No multi-stage build** — development tools, compilers, and test runners included in the production image.
- **No `HEALTHCHECK` instruction** — the container reports healthy immediately regardless of app readiness.

### Infrastructure-as-code anti-patterns

**DO NOT default to:**

- **Hardcoded environment names, regions, and resource sizes** in Terraform/CloudFormation with no variables — impossible to reuse across environments.
- **No remote state backend** — Terraform state stored locally.
- **`terraform apply` without plan review** in an automated pipeline.
- **All infrastructure in a single monolithic file** — `main.tf` with 2,000 lines.
- **`0.0.0.0/0` ingress rules** on ports that should only be accessible from within a VPC.
- **No log retention policy** — logs accumulating indefinitely.

**For every infrastructure or pipeline file generated, state what the production environment, team size, and deployment frequency are. If those are unknown, say so — do not generate a generic YAML and call it production-ready.**

---

## Documentation & Content

### Documentation anti-patterns

**DO NOT default to:**

- **README that describes what the project is without explaining how to use it** — feature paragraphs, badge row, one-line install command, nothing else.
- **Installation instructions that assume a clean machine** — no mention of required Node/Python version, system dependencies, or environment variable configuration.
- **No "Getting Started" path distinct from "Full API Reference"** — everyone dumped into the same flat structure.
- **Code examples with only the happy path** — no error handling, no 401 path, no edge case.
- **Changelog entries that say "Bug fixes and performance improvements"** with no specifics.
- **API documentation that only lists parameters** without explaining when to use the endpoint, preconditions, and caller responsibilities.

### Content strategy anti-patterns

**DO NOT default to:**

- **"2 posts per week" publishing cadence** without knowing whether the audience reads that much or whether there's original material to sustain it.
- **Topic selection by keyword volume alone** — writing whatever has the highest search volume regardless of genuine team expertise.
- **Case studies that describe what was done with no outcome** — "We helped Company X redesign their dashboard" with no before/after metric.
- **Video transcripts auto-published as blog posts** — spoken-word grammar is not written-word grammar.

---

## Cross-Discipline Code Quality

These failures cut across every technical discipline:

- **God components / god functions** — one React component or function handling data fetching, business logic, formatting, error handling, and rendering simultaneously.
- **No error boundaries in React trees** — one component failure brings down the entire UI with a white screen.
- **No environment variable validation on startup** — the app starts, runs fine for 10 minutes, then fails with a cryptic error that has nothing to do with the root cause.
- **`git commit -m "fix"` or `git commit -m "update"`** — no context, no scope, no history.
- **`^major.minor.patch` in `package.json`** — the same `npm install` produces different results six months later.
- **No `.nvmrc` or `engines` field** — the required Node version is documented nowhere.
- **Tests designed to pass, not to catch regressions** — only the happy path.
- **Copy-pasted code across three files** with slight variations — three identical bugs when the logic needs to change.
- **Over-engineered abstractions for a project not yet large enough to need them** — microservices for a solo-developer project, a design system for a four-page site.

---

## When the User Pushes Back

If the user says "this still looks AI-generated," "this is generic slop," or "a junior could have written this":

**Do not**: Adjust spacing. Change a color. Swap one icon for another. Add more sections.

**Do**: Name the specific item from above that you defaulted to. State it explicitly — "I defaulted to [pattern]. The replacement is [specific, justified alternative]." Then rebuild from that decision, not from the previous draft with surface changes.

The difference between a 40-year practitioner and a model generating defaults is not technique. It is the willingness to discard a draft that has no specific reason to exist.