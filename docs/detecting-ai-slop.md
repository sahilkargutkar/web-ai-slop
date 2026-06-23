# Is This Site AI-Generated? A Practitioner's Detection Guide

> A field guide for designers, developers, content strategists, UX researchers, and DevOps engineers to identify AI-generated web output. Written from 40+ years of combined practitioner experience across every web discipline.

---

## How to Use This Guide

Open the site. Work through each section that applies to your discipline. Each item is a confirmed tell — a pattern so statistically common in AI-generated output that its presence is evidence, not coincidence.

**Scoring**: Count the matching items per section.

| Matches | Verdict |
|---|---|
| 0–1 per section | Probably human-made, or well-reviewed AI output |
| 2–3 per section | AI-assisted with minimal editing |
| 4+ per section | Generated and shipped without review |
| 4+ across multiple sections | Fully AI-generated, likely in a single session |

These are not rules about whether AI was used. They are rules about whether any human with professional judgment reviewed and edited the output before shipping.

---

## Section 1 — Visual Design Tells

Open the site. Before reading anything, look at it. These are the patterns you'll notice in the first 10 seconds.

### 1.1 The Hero Section

- [ ] **Purple-to-blue or purple-to-pink radial gradient blob** behind the headline — a large, soft, glowing aurora-style background blur, typically centered or offset in the top-right quadrant.
- [ ] **Centered layout: logo → headline → subheadline → two pill-shaped CTA buttons → browser-mockup screenshot** — in that exact order, with nothing else above the fold.
- [ ] **100vh hero with only text and a button** and no other content — treating whitespace as sophistication rather than as a design decision.
- [ ] **A floating laptop, phone, or dashboard screenshot** rotated slightly or rendered in a device mockup frame — the only visualization of what the product actually does.
- [ ] **"Trusted by" logo strip** immediately below the hero, with logos grayscaled, all at the same height, evenly spaced in a single row.

### 1.2 Decorative Elements

- [ ] **Particle network animation** — small dots connected by faint lines, either static or slowly moving. Used as the background or in a dedicated "AI" or "technology" section.
- [ ] **Wavy SVG divider** between two sections — an organic curve used as a section separator, typically going from white to a light gray or brand color.
- [ ] **Blob-shaped decorative SVG** — an irregular, amorphous shape used as a background accent, usually in the brand's primary color at low opacity.
- [ ] **Isometric illustration of a laptop, rocket, or office worker at a desk** — stock-style 3D illustration used as hero art with no relationship to the actual product.
- [ ] **Abstract low-poly mesh or geometric triangle pattern** as a background texture.
- [ ] **Neon/glowing outer-glow shadow** on a card, button, or image — a colored box-shadow in the brand's primary color, applied to multiple elements simultaneously.
- [ ] **Dashboard widget collage** used as decorative background — a wall of small charts, graphs, and stats tiles arranged as visual wallpaper to imply "data-driven."

### 1.3 Cards and Components

- [ ] **Glassmorphism feature cards** — frosted-glass effect with `backdrop-filter: blur`, a 1px semi-transparent white border, and subtle inner glow. Used as the default "premium" card style for all content regardless of what the card contains.
- [ ] **Bento grid of feature cards** — a CSS grid of rounded-corner cards, each containing an icon in a rounded square, a short bold title, and exactly 1–2 sentences of copy. All cards the same height.
- [ ] **Every button is a pill shape** — `border-radius: 9999px` applied uniformly. No variation between primary, secondary, and tertiary button styles.
- [ ] **Every card has excessive border-radius** — 16px, 20px, or higher on cards, inputs, and image containers as a blanket stand-in for "friendly."
- [ ] **Glowing primary-color button** — the main CTA button has a colored drop shadow matching the button's background color, making it appear to emit light.
- [ ] **Icon on every single feature, nav item, and card** — icons used not for scannability but to "fill in" the visual space and make the page look complete.

### 1.4 Page Rhythm and Layout

- [ ] **Identical section-rhythm top to bottom**: full-width colored section → white section → full-width colored section → white section, with no variation in density or pacing.
- [ ] **Every section centers its content** in a single-column or two-column layout — no asymmetric compositions, no edge-to-edge content, nothing breaking the grid deliberately.
- [ ] **Symmetrical 3-column or 6-column feature grid** — features arranged in groups of 3 or 6 because those feel "balanced," not because that's how many features exist.
- [ ] **Footer with 4–5 link columns** containing the same 20–30 links regardless of whether this product's users would ever navigate any of them.
- [ ] **Sticky navigation on a one-scroll landing page** where the nav competes with the content for the user's attention.

---

## Section 2 — Color and Typography Tells

### 2.1 Color

- [ ] **Primary brand color is purple/violet (#7c3aed or similar) or indigo** with no clear brand rationale for the choice — just the default "tech" palette.
- [ ] **Pure `#000000` background** or **pure `#ffffff` background** — no warmth, coolness, or tonal consideration. The white feels clinical; the black feels harsh.
- [ ] **Dark mode as the only or default option** — chosen because dark mode "feels premium" in a demo, not because the product's users or content benefit from it.
- [ ] **Gradient used on the primary CTA button** when nothing else in the design uses gradients — an isolated gradient button signals AI because it is the AI default for "making the button stand out."
- [ ] **Five or more distinct accent colors** used across cards, icons, badges, and section backgrounds on a single page — "vibrant" interpreted as "many colors."
- [ ] **Colors with no stated rationale** — the palette cannot be explained by the brand category, target audience, or competitive positioning. They just appeared.

### 2.2 Typography

- [ ] **Inter is the only typeface** — no display face for large headlines, no serif for editorial contrast, no consideration of whether Inter serves this specific brand.
- [ ] **All font weights are 400, 600, and 700** — the three default weights, nothing else.
- [ ] **Large headline has default letter-spacing** — at 48px or higher, the tracking has not been tightened. Professional type systems use `letter-spacing: -0.02em` to `-0.05em` on display sizes. Un-tightened large text is a reliable AI tell.
- [ ] **No tonal hierarchy in body text** — all body copy, captions, labels, and meta text are the same color, differentiated only by font size. Real type systems have at least 3 tonal levels: primary text, secondary/muted, and faint/disabled.
- [ ] **Line-height is the same on all text sizes** — `1.5` applied uniformly from 12px captions to 56px headlines. Captions need tighter leading; display text needs even tighter.
- [ ] **Bold is the only emphasis mechanism** — no italic, no small-caps, no color shift for in-text emphasis. Everything is either regular or bold.
- [ ] **All-caps labels on every small text element** — ALL CAPS used as a typographic hierarchy shortcut on section labels, card labels, and badges, regardless of whether the brand uses it.

---

## Section 3 — Copywriting Tells

Read the page text out loud. These patterns are audible once you know what to listen for.

### 3.1 Headline Patterns

- [ ] **"Unlock/Unleash/Elevate/Supercharge/Empower your [noun]"** — verb of vague empowerment + possessive + abstract noun. The most over-trained grammatical slot in SaaS copy. Examples: "Unlock your team's potential." "Supercharge your workflow." "Elevate your brand."
- [ ] **Rule-of-three adjective stack as the headline or subheadline**: "Fast. Reliable. Secure." / "Simple. Powerful. Flexible." / "Bold. Human. Connected." — three one-word sentences separated by periods. This is the AI's attempt at punchy copy. It communicates nothing specific.
- [ ] **Em-dash sentence that states the same thing twice**: "We don't just build software — we build the future of work." / "This isn't just a tool — it's your competitive advantage." The second half of the em-dash adds zero new information.
- [ ] **"[Product]: The [adjective] way to [do thing]"** as the page title — the most common AI headline template.
- [ ] **"In today's [fast-paced / digital / competitive / ever-changing] world..."** — the throat-clearing opener. Any sentence that begins by establishing the context of the era is filler.

### 3.2 Body Copy Patterns

- [ ] **"Whether you're a [X] or a [Y], [Product] has you covered"** — the faux-inclusive sentence that tries to address every audience and addresses none of them.
- [ ] **"Say goodbye to [pain point]"** — written as if the pain point is a character departing a scene.
- [ ] **"Built for teams of every size"** or **"Scales with your business"** — the hedge that avoids making a specific claim about who the product is for.
- [ ] **"Designed with [audience] in mind"** — passive-voice construction that implies intentionality without demonstrating it.
- [ ] **Bulleted feature list where every line begins with the same gerund**: "Streamline your...", "Automate your...", "Optimize your...", "Accelerate your..." — gerund + "your" + noun, 6–8 times.
- [ ] **"Trusted by 10,000+ teams"** or **"Loved by developers worldwide"** — unattributed statistics with no source, no named customer, no verification, used as visual filler.
- [ ] **"Intuitive," "seamless," "powerful," "robust," "best-in-class"** used as adjectives without any evidence — words that have been used so often in AI copy that they are now meaningless noise.

### 3.3 Structural Content Patterns

- [ ] **Page title is "Home | [Product Name]"** or **"[Product Name] | The [adjective] [category] platform"** — no specific value proposition in the title tag.
- [ ] **"Our Story" or "About Us" section** that follows this template: year founded → problem we noticed → mission statement → "passionate team" → vague claim about impact.
- [ ] **FAQ section that answers questions nobody asked**: "What is [Product]?", "How do I sign up?", "Is there a free trial?" — written to pad the page, not to address real objections.
- [ ] **Testimonials from "J.D., Marketing Manager"** — circular stock-photo avatar, first initial + last initial or first name + last initial, job title without company name, one-sentence quote that contains no specific number, outcome, or named feature.
- [ ] **CTA button copy that says "Get Started," "Learn More," or "Try Free"** — not specific to what clicking the button does or delivers.
- [ ] **Section headers that are vague nouns**: "Features," "Solutions," "Benefits," "Why Us," "How It Works" — not claims, not promises, just category labels.
- [ ] **Blog post introduction that opens with a rhetorical question**: "Have you ever wondered why [generic problem]?" — a technique AI uses to establish relevance before making any actual point.

---

## Section 4 — UX and Information Architecture Tells

Navigate the site as a user would. These are the patterns that reveal no one modeled actual user behavior.

### 4.1 Page and Section Structure

- [ ] **The site follows this exact section sequence**: Hero → Logo strip → Features (3 or 6 cards) → "How It Works" (3 steps, numbered, with an icon each) → Testimonials → Pricing (3 tiers) → FAQ accordion → Final CTA banner → Footer. Every page, every product.
- [ ] **"How It Works" has exactly 3 steps** regardless of how many steps the process actually takes. Step 1: Sign up. Step 2: [Do the main thing]. Step 3: Achieve vague outcome.
- [ ] **Pricing section has exactly 3 tiers**: Starter / Pro / Enterprise (or Basic / Business / Scale). The middle tier is highlighted with a colored border and the badge "Most Popular" — without any data indicating it is actually the most popular.
- [ ] **The "Enterprise" tier's price field says "Contact us"** on a product that has no enterprise features and no enterprise customers.
- [ ] **Navigation items mirror internal company departments** rather than user tasks: "Product / Solutions / Resources / Company" — not "Find a template / Run a campaign / See pricing."

### 4.2 Interaction and State Design

- [ ] **Empty states say "No [items] found"** with no explanation of what items are, how to create one, or what the user should do next.
- [ ] **Error messages say "Something went wrong"** or "An error occurred. Please try again." — no specificity about what happened or what the user can do about it.
- [ ] **Every hover state is an opacity reduction** — `opacity: 0.7` or a lighter version of the element's color. The same affordance for buttons, links, cards, icons, and images.
- [ ] **Scroll-triggered animations on every section** — content slides up or fades in uniformly as you scroll, applied to every section regardless of whether the content benefits from the reveal.
- [ ] **No loading states or skeleton screens** — content either appears instantly or a spinner shows with no intermediate state.
- [ ] **A modal dialog appears for a trivially reversible action** — confirming deletion of a single tag, or confirming a "start free trial" action that has no immediate consequence.

### 4.3 Accessibility (Inspect with a Screen Reader or DevTools)

- [ ] **Focus styles are removed** — tabbing through the page produces no visible focus ring on interactive elements. Styled away because it "looked ugly."
- [ ] **Images have no `alt` text**, or `alt` text that repeats the filename (`image_final_v3.png`) or just says `"image"`.
- [ ] **Icon-only buttons have no accessible label** — a trash-can or close icon with no `aria-label`, `aria-describedby`, or visually-hidden text.
- [ ] **Form inputs have no `<label>`** — only placeholder text, which disappears when the user starts typing and provides no persistent description.
- [ ] **Heading levels are skipped** — the page jumps from `<h1>` to `<h3>` because the `<h3>` style matched the visual design. The document outline is broken.
- [ ] **Animations have no `prefers-reduced-motion` media query** — no way for users with vestibular disorders or motion sensitivity to opt out.

---

## Section 5 — Source Code Tells

Open DevTools. View page source. These patterns are readable in the HTML, CSS, and JavaScript of the page.

### 5.1 HTML Tells

- [ ] **`<title>` is the framework default**: "React App," "Vite App," "Create Next App," or "[Product Name]" with no description.
- [ ] **No `<meta name="description">`** or a meta description that reads as a product brochure rather than a specific, search-indexed answer.
- [ ] **No `lang` attribute on `<html>`** — `<html>` with no language specified.
- [ ] **Entire page structure is `<div>` soup** — no `<main>`, `<nav>`, `<header>`, `<footer>`, `<article>`, `<section>`, `<aside>`. Every element is a `<div>` or a `<span>`.
- [ ] **`<br><br>` used between paragraphs** instead of `<p>` elements with margin.
- [ ] **`alt=""` is absent** from images that are not purely decorative.
- [ ] **Link text is "click here," "read more," or "learn more"** instead of descriptive text.
- [ ] **`<button>` contains only an SVG icon** with no text, no `aria-label`, no accessible name.

### 5.2 CSS Tells

- [ ] **`transition: all 0.3s ease`** applied to every interactive element — one easing curve, one duration, covering every property that could animate. Found on `.btn`, `.card`, `.nav-link`, `.icon`, all with identical values.
- [ ] **`z-index: 9999`** (or `999` or `99999`) on multiple elements — used as a blunt override rather than a defined stacking context.
- [ ] **Magic numbers throughout** — `margin-top: 37px`, `padding: 13px 22px`, `gap: 17px` — values with no relationship to a spacing system.
- [ ] **No CSS custom properties** (`--color-*`, `--spacing-*`) — color values, font sizes, and spacing values are hardcoded literals repeated across hundreds of rules.
- [ ] **`px` units for all font sizes** — `font-size: 16px`, `font-size: 14px` — no `rem` or `em`, preventing browser font-size preferences from taking effect.
- [ ] **`!important` used more than once** — specificity conflicts resolved by escalation rather than by fixing the structure.
- [ ] **Media queries at exactly 768px and 1024px** — arbitrary breakpoints that correspond to "what phones and tablets are" rather than to where the content actually breaks.
- [ ] **No `max-width` on body text** — paragraph text spans the full container width at all viewport sizes, reaching 1400px or more on wide monitors.

### 5.3 JavaScript Tells

- [ ] **`console.log` statements in production** — visible in the browser console during normal page use.
- [ ] **No error handling on `fetch()` calls** — inspect network requests; when one fails, the page silently shows nothing rather than an error state.
- [ ] **`setTimeout(() => ..., 300)`** or similar — artificial delays used as a substitute for real loading state management.
- [ ] **`localStorage` or `sessionStorage` keys with generic names** like `"data"`, `"user"`, `"token"` — no namespace, no collision prevention.
- [ ] **The entire application in one JavaScript bundle** with no code splitting — a single `bundle.js` or `main.js` file exceeding 1MB downloaded on initial load.

### 5.4 Performance Tells (Lighthouse / Network Tab)

- [ ] **Full-resolution JPEGs or PNGs served at display size** — a 3000×2000px image rendered at 400×267px, with no `srcset`, no WebP version, no `loading="lazy"` on below-fold images.
- [ ] **Google Fonts loaded for all weights** — the `<link>` preload includes weights 100, 200, 300, 400, 500, 600, 700, 800, 900 when only 400 and 700 are ever used.
- [ ] **No `font-display: swap`** — text is invisible for several hundred milliseconds while the web font loads (Flash of Invisible Text).
- [ ] **Third-party chat widget, analytics, and A/B testing script all load synchronously before the page renders** — three render-blocking scripts in `<head>` for tools that don't need to run until the page is interactive.
- [ ] **Lighthouse Performance score below 50 on mobile** — not a specific AI tell, but AI-generated code that hasn't been reviewed routinely scores here.

---

## Section 6 — Infrastructure and DevOps Tells

These require access to the repository, CI/CD pipeline, or infrastructure configuration. Relevant for teams reviewing internal AI-generated scaffolding.

### 6.1 CI/CD Pipeline

- [ ] **3-stage pipeline: build → test → deploy** applied as the universal template, regardless of whether the project has any tests, multiple deployment targets, or any deployment strategy beyond "push main."
- [ ] **`on: push` triggers on every branch** with no branch filtering — every developer branch triggers a deploy pipeline.
- [ ] **Secrets written directly into the YAML file**: `API_KEY: "abc123_hardcoded"` — not referenced from GitHub Secrets, AWS Parameter Store, or Vault.
- [ ] **`npm install` in CI** instead of `npm ci` — non-deterministic; may install different package versions than the lockfile specifies.
- [ ] **No dependency caching** — every pipeline run downloads the full `node_modules` from scratch.
- [ ] **No staging environment** — the pipeline deploys directly to production on merge to main, with no intermediate verification step.

### 6.2 Dockerfile

- [ ] **`FROM node:latest`** — the `latest` tag pulls a different image over time, breaking reproducibility silently.
- [ ] **No `USER` instruction** — the container runs as root.
- [ ] **`COPY . .` appears before `npm install`** — every source file change invalidates the dependency layer cache, forcing a full reinstall on every build.
- [ ] **No `.dockerignore`** — `node_modules/`, `.git/`, test files, and `.env` files are copied into the image.
- [ ] **Image size exceeds 1GB** — development tools, compilers, and test frameworks included in the production image. No multi-stage build.
- [ ] **No `HEALTHCHECK` instruction** — the container reports healthy immediately, before the application has actually started and is serving traffic.

### 6.3 Infrastructure as Code

- [ ] **Hardcoded region names, instance sizes, and environment labels** — `"us-east-1"`, `"t3.micro"`, `"production"` as string literals with no variables, making the config impossible to reuse across environments.
- [ ] **No remote Terraform state backend** — `terraform.tfstate` committed to the repository, or stored only locally.
- [ ] **All resources in a single `main.tf`** exceeding 500 lines — networking, compute, databases, IAM, and logging in one file with no module boundaries.
- [ ] **Security groups with `0.0.0.0/0` ingress** on ports that should be internal — database ports, admin ports, or API ports accessible from the public internet.
- [ ] **No resource tagging strategy** — cloud resources with no `Owner`, `Environment`, `Project`, or `CostCenter` tags.

---

## Section 7 — Documentation Tells

Read the README, API docs, and changelog.

- [ ] **README describes the project but not how to use it** — paragraphs about what it is, a badge row, one installation command, and nothing else.
- [ ] **Installation instructions assume a clean machine** — no mention of required Node/Python/Ruby version, no mention of required environment variables, no mention of system-level dependencies.
- [ ] **No "Getting Started" guide distinct from the API reference** — first-time users and experienced users are directed to the same flat documentation.
- [ ] **Code examples only show the happy path** — no error handling, no rate limit handling, no "what to do if this returns a 401" section.
- [ ] **Changelog entries that say "Bug fixes and performance improvements"** — no specifics, no issue references, no version-tagged changes.
- [ ] **API documentation that only lists parameters and types** — no explanation of when to call the endpoint, what state must be true before calling it, or what the caller is responsible for afterward.
- [ ] **Blog post introductions that open with a rhetorical question** the target reader did not have — "Have you ever wondered why CI pipelines are so slow?"
- [ ] **"Our Story" or "About" page** that reads: founded in [year], we noticed [problem], our mission is to [vague positive change], our team is passionate, we serve customers worldwide.

---

## The Master Swap Test

After reviewing the site, perform this final check:

**Replace the product name with a competitor's name throughout the copy. Does the site still make complete sense?**

If yes — if the headline, the subheadline, the feature descriptions, the testimonials, and the CTAs would all work verbatim for any other product in the same category — the copy was generated without any specific knowledge of what makes this product different. That is the definitive marker of AI-generated content that was not reviewed by someone with domain knowledge.

A human writer with domain expertise writes at least one sentence that is so specific to this product that it could not be said about any other. That sentence is the proof of authorship.

---

## Quick Reference — Top 10 Highest-Confidence Tells

If you see any three of these together, the site was almost certainly AI-generated and shipped without professional review:

1. **Purple aurora gradient blob behind the hero headline**
2. **Bento grid of rounded-square icon cards with "Fast. Secure. Scalable."**
3. **"Unlock your [noun]" or "Supercharge your [noun]" headline**
4. **Rule-of-three adjective stack ("Simple. Powerful. Flexible.")**
5. **Testimonials: circular avatar, first name + last initial, no specific outcome**
6. **3-tier pricing with "Most Popular" highlighted on the middle tier**
7. **`transition: all 0.3s ease` on every interactive element in the CSS**
8. **Inter in 400/600/700 with default letter-spacing on large headlines**
9. **"How It Works" with exactly 3 generic steps**
10. **No `alt` text on images, no `lang` on `<html>`, `<title>` is the framework default**

---

*This guide is part of the [web-ai-slop](https://github.com/sahilkargutkar/web-ai-slop) skill package. Contributions welcome — open a PR with a pattern that belongs on this list.*
