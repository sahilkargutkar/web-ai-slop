---
name: web-ai-slop
description: "Filters web output against a multi-discipline checklist of AI default patterns. Use before shipping any design, copy, UI code, infrastructure config, or documentation. Trigger when the user asks for something 'premium' or 'not AI-looking', when you're about to reach for a glowing gradient, bento grid, SaaS empowerment copy, a 3-tier pricing section, a 3-stage CI/CD YAML, or a god component."
---

# Web AI Slop — The Practitioner's Anti-Default Checklist

A trained filter, not a style guide. This skill exists because language models converge on the same small set of "safe" defaults across every web discipline — not because those defaults are good, but because they are the statistical center of the training data. The job of this skill is to name that center precisely so you can deliberately step away from it.

**Rule of application:** Draft your output first. Then run it against the relevant sections below. If you match **2 or more items in any single section**, you have not made a decision — you have defaulted. Discard the draft and make a specific, justified choice for this product, team, and context.

Apply this filter silently. Do not narrate "I'm checking this against my anti-slop list" to the user.

---

## Section 1 — Visual Design (Web Designer / UI Designer perspective)

These are the patterns a designer with 40 years of craft knowledge would immediately identify as machine output.

### 1a. Layout and composition defaults

- **Centered hero, headline + subhead + two pill CTA buttons + browser-mockup screenshot below the fold** — treated as the only possible layout, applied to every product regardless of what that product actually is. This is a starting skeleton, not a decision.
- **Symmetrical 3-column or 6-column feature grids** — every section resolves to three items or six items arranged identically, because three and six feel "balanced" to a model without knowledge of the actual feature set.
- **Full-viewport hero sections with nothing but text, a subheadline, and a button** — 100vh of empty air treated as sophistication.
- **Section → divider → section → divider rhythm with no variation** — every page breathes the same. Real page rhythm varies: compressed detail sections, open breathing sections, dense data sections.
- **Sticky navigation that appears on every page** regardless of whether the page is a one-scroll landing page, a long-form article, or an app view where navigation competes with content.
- **Footer with 4–5 column link columns** containing links that nobody using this specific product would realistically navigate to.
- **Icons for features that don't require icons** — AI models love to put a Lucide or Heroicon next to every feature, even when it doesn't add clarity.DOnt use emoji's for icons in any page , dont use emojis at all in the website, instead use actual icons.You can ask which icons user prefer, and based on user input select them.dont use the default icon themes of shadcn ui, make your own or use a library of icons that user prefers.


### 1b. Decorative motifs

- **Glowing gradient blob / aurora background** — purple-to-blue or purple-to-pink radial blur behind a hero. The single most common AI default for "modern tech company." Any senior designer who sees this in a brief sighs audibly.
- **Particle network / floating dots with connecting lines** — the visual shorthand for "AI" or "data." If the brief mentions AI, the particle globe or neural-net mesh is the first output — therefore it is the wrong output.
- **Wavy or blob SVG section dividers** — organic curves between sections applied indiscriminately to signal "approachable tech" without any brand reason.
- **Glowing brand-color halos / outer-glow shadows** on cards, buttons, or images — the neon-border trick applied to everything at once.
- **Tiling small dashboard widgets and charts as decorative background wallpaper** — a busy placeholder that stands in for a real product decision. The "particle network" of 2025/26.
- **Isometric 3D illustrations of laptops, rockets, or people-at-desks** as stock hero art when the brief gave no instruction.
- **Abstract geometric low-poly backgrounds** with faint triangular meshes or hexagons used as texture.
- **Floating UI element screenshots positioned at an angle** ("device mockup" shot) as the only form of product visualization considered.

### 1c. Component-level tells

- **Glassmorphism cards** — frosted-glass translucent panels with a soft white border and `backdrop-filter: blur()` applied as default "premium" card style regardless of what the card contains or the brand it represents.
- **Bento grid of icon-in-rounded-square feature cards**, each containing a Lucide or Heroicon and exactly three lines of generic benefit copy ("Fast. Secure. Scalable.").
- **Excessive border-radius on everything** — cards, buttons, inputs, images, all at 16px or higher as a catch-all stand-in for "friendly."
- **Every button a pill shape** (`border-radius: 9999px`) regardless of whether the brand calls for it.
- **Testimonial carousel with stock-photo circular avatar, first name + last initial, and a generic one-line quote** that contains no specific number, outcome, or named feature.
- **Pricing section always 3 tiers, always with the middle one highlighted** by a colored border and the label "Most Popular," regardless of whether that framing serves this product.


### 1d. Quick-scan signal table

Open the site and look at it for 10 seconds before doing anything technical. These are the signals visible without inspecting code.

| Signal | What to look for |
|---|---|
| **The purple/blue gradient** | Many AI tools default to the same blue-to-purple gradient — once you've seen it, you can't unsee it. Usually a radial blur behind the hero. |
| **Glassmorphism everywhere** | Frosted-glass cards with white borders, used as the default "premium" treatment regardless of brand. |
| **Particle networks / neural-net visuals** | Floating dots with connecting lines as generic shorthand for "AI" or "data," with no specific referent to what the product does. |
| **Bento grid of icon cards** | 3 or 6 rounded-square cards, each with a Lucide/Heroicon and 2–3 lines of generic benefit copy. |
| **Inconsistent spacing** | Margins and padding vary between sections, so the page rhythm feels uneven — consistent spacing is one of the clearest signs of considered design, and its absence is a tell. |
| **Weak typographic hierarchy** | Default fonts, awkward line lengths, inconsistent heading sizes, and cramped line spacing all point to type that was never properly set. |
| **Poor contrast** | Light grey text on white, or weak text/background contrast — WCAG sets a 4.5:1 minimum contrast ratio for normal text, and many AI-default palettes don't clear it. |
| **Identical card hover effects everywhere** | Every card lifts or glows the same way on hover, applied uniformly rather than where it adds real affordance. |
| **Excessive sparkle/AI emoji** | ✨ used liberally in headlines and buttons as a visual signal for "AI-powered," now itself a tell. |

**Quick test:** Resize the browser narrower, or open on a phone. AI-generated layouts often break, overlap, or overflow at screen sizes the model was never specifically prompted to handle — real responsive QA across breakpoints is one of the first things skipped.

**Instead:** Pick ONE real visual device — a specific illustration, a diagram of the actual product's data flow, a screenshot of the real interface — render it with restraint, and give it room. A company that ships serious product puts one precise idea per screen, not a collage of AI-default textures.


---

## Section 2 — Color & Typography (Web Designer / UI Designer perspective)

### 2a. Color defaults

- **Purple/violet (#7c3aed-ish) or indigo paired with blue or pink** as the automatic "tech" palette when the brand has given no signal pointing to it.
- **Pure black (#000000) or pure white (#ffffff) backgrounds** instead of a considered near-black or near-white that carries slight warmth, coolness, or character.
- **The "dark mode by default" decision made for aesthetic reasons** — because dark mode photographs well in a demo or feels premium — rather than because the content, context, or user base calls for it.
- **Gradient buttons as the primary CTA style** without any rationale for why this brand would use gradients.
- **Five or more accent colors in a single design system** because "vibrant" was the brief word — real systems are built on restraint; one accent, one functional palette, one semantic palette.
- **Color choices that have no provenance** — the hex values appeared in the response without any explanation of why this product's brand, category, or audience informed them.

### 2b. Typography defaults

- **Inter in weights 400, 600, and 700 only**, with no display typeface for headlines, no serif for body contrast, and no consideration of whether Inter is the right choice for this brand.
- **Letter-spacing untouched at `letter-spacing: 0`** on large display headlines — professional type systems tighten tracking (`letter-spacing: -0.02em` to `-0.05em`) as point size increases. Default tracking on a 72px headline looks like a template.
- **No visual type hierarchy beyond size and weight** — body, muted, and faint text all at the same color value, differentiated only by font-size. Real hierarchies use at least three tonal steps.
- **Line-height not considered per context** — same `line-height: 1.5` on a 12px caption and a 56px headline.
- **All-caps labels on everything** as a substitute for typographic hierarchy thinking.
- **Font-weight 700 ("bold") as the only emphasis tool** in body copy, never italic, never small-caps, never color-based emphasis.

**Instead:** Derive the palette from a concrete source — the product category, a specific competitor you are deliberately differentiating from, or a single brand constraint given by the client. State the hex values and their rationale before using them. State which typeface and why before specifying it.

---

## Section 3 — Copywriting & Content Strategy (Content Developer perspective)

These are the patterns that a 40-year editorial professional or senior UX writer would immediately flag in a content review.

### 3a. Sentence-shape clichés

- **"In today's fast-paced/digital/ever-changing world..."** — any throat-clearing opener that establishes context instead of stating a claim.
- **"Unlock/Unleash/Elevate/Supercharge/Empower your [noun]."** — verb-of-vague-empowerment + possessive + abstract noun. This is the single most over-trained grammatical slot in SaaS marketing copy.
- **"Whether you're a [X] or a [Y], [Product] has you covered."** — the faux-inclusive opener.
- **"Say goodbye to [pain point]."** — written as if the pain point is a character leaving a party.
- **"Built for teams of every size."** or "Built for [speed/scale/teams] at every level."
- **Em-dash sentences that restate the same claim twice** — "We don't just build software — we build the future of work." The second half adds no information.
- **Rule-of-three adjective stacks**: "Fast. Reliable. Secure." / "Simple. Powerful. Flexible." / "Bold. Human. Connected." Three one-word sentence fragments separated by periods. Every SaaS company has this. None of them mean anything.
- **"Trusted by [N]+ teams/companies/developers"** with no source, no named company, and no context — used as visual filler, not as evidence.
- **Bulleted feature lists where every line begins with the same gerund** — "Streamline your workflows. Automate your pipelines. Optimize your delivery." Gerund + possessive noun, repeated for 6–8 bullets.
- **"Designed with [audience] in mind"** — the passive-voice hedge that avoids making a specific claim.

### 3b. Structural content defaults

- **Generic page titles** like "Home | Product" or "About Us | Company" that tell search engines and users nothing specific.
- **Meta descriptions that read like a product brochure** rather than a specific, useful answer to a user's search intent.
- **"Our Story" or "About Us" copy that reads like a LinkedIn summary** — founded in year, mission to disrupt, passionate team, world-class product.
- **Blog post introductions that begin with a question** the reader did not have: "Ever wondered why [generic industry problem]?"
- **Section headers phrased as vague nouns** ("Features," "Solutions," "Why Us," "Get Started") rather than claims or specific promises.
- **CTA button copy that only says "Get Started," "Learn More," or "Try Free"** — not specific to what the action actually does or delivers.
- **FAQ content that answers no real objections** — questions invented to pad the page ("What is [Product]?" "How do I get started?") rather than the real questions from sales calls.
- **Social proof from fictional or unnamed companies** ("Leading companies trust us") rather than earned, attributed, specific testimony.

### 3c. Tone and voice defaults

- **Writing in a "professional" register that strips all personality** — flat, inoffensive, interchangeable with any other company in the category.
- **Addressing the user as "you" while writing about them as if they are a persona abstraction** ("Teams like yours need...") rather than a person with a specific problem.
- **Using "seamless," "intuitive," "powerful," or "robust"** as adjectives without any specific evidence — these words have been used so often that they communicate nothing except that the writer had no more specific thing to say.
- **Active voice mimicry without subject clarity** — "Enabling teams to ship faster" has no grammatical subject. Who enables? What ships? Faster than what?

**Instead:** Write one sentence that only makes sense for this specific product — a sentence that a competitor could not copy-paste into their own website without it being obviously wrong. If the company name can be swapped out and the sentence still works, delete it.

---

## Section 4 — UX Design & Information Architecture (UX Designer perspective)

These are the patterns that a 40-year UX researcher or information architect would flag in a heuristic review.

### 4a. Page and flow structure defaults

- **Every landing page follows the identical section sequence** — Hero → Logo strip → Features (3 or 6 cards) → How It Works (3 steps) → Testimonial carousel → Pricing (3 tiers) → FAQ accordion → Final CTA banner → Footer — applied to every product without asking whether this sequence serves this specific conversion goal.
- **"How It Works" sections with exactly 3 steps, each numbered** regardless of how many steps the actual process takes.
- **Onboarding flows with a progress bar at the top and no skip option** — the default "wizard" pattern applied to every registration flow without considering whether the user actually needs to complete all steps before getting value.
- **Empty states that just say "No items found"** without explaining what items are, how to create one, or what the user should do next.
- **Error messages that say "Something went wrong"** or "An error occurred" with no actionable next step and no indication of what caused the problem.
- **Forms with no inline validation**, all errors appearing only after submit, all at once, at the top of the form.
- **Modal dialogs for every confirmation action** — including for actions that are trivially reversible, where a toast or inline toggle would be less disruptive.
- **Navigation items that mirror the company's internal department structure** rather than the user's mental model of the tasks they are trying to complete.
- **Breadcrumbs generated for every page** regardless of whether the site is shallow enough that breadcrumbs add no navigational value.

### 4b. Interaction design defaults

- **Every hover state is an opacity reduction or color lightening** — `opacity: 0.7` or a tint of the base color — without considering whether the element needs a different affordance signal.
- **Focus styles removed or suppressed** because they "look ugly" — accessibility failure disguised as aesthetic preference.
- **Scroll-triggered animations on every section** — elements sliding up, fading in, or scaling on scroll applied uniformly because it "feels dynamic," regardless of whether motion serves the content.
- **Infinite scroll with no option to return to position** — applied to every list because pagination feels "old."
- **Hamburger menus on tablet breakpoints** where there is sufficient horizontal space for visible navigation.
- **Click targets smaller than 44×44px** on mobile — the single most common mobile usability failure, and the most avoidable.
- **No loading states or skeleton screens** — content appears or a spinner shows, with nothing in between.
- **Tooltips as the only way to access critical information** — information hidden behind hover states is inaccessible on touch devices.

### 4c. Accessibility defaults (the ignored discipline)

- **Color contrast ratios not checked** — text color and background color chosen for aesthetics without verifying WCAG 2.1 AA (4.5:1 for normal text, 3:1 for large text).
- **Images with no `alt` text**, or `alt` text that just repeats the filename or says "image."
- **Icon-only buttons with no accessible label** (`aria-label` missing) — a button that is visually a trash-can icon has no meaning to a screen reader user.
- **Form inputs without associated `<label>` elements** — placeholder text used as a substitute for a label, which disappears when the user starts typing.
- **`<div>` and `<span>` used as interactive elements** with click handlers but no `role`, no `tabindex`, and no keyboard event handler.
- **Heading levels skipped** — jumping from `<h1>` to `<h3>` because the `<h3>` style looked right, breaking document structure for screen readers.
- **No `skip to main content` link** for keyboard users who would otherwise have to tab through an entire navigation on every page.
- **Animations with no `prefers-reduced-motion` media query** — users with vestibular disorders, epilepsy, or motion sensitivity cannot opt out.
- **Tailwind css** - dont use tracking in any className with tracking-wider or tracking-tight etc. Do not use uppercase letters in any text.Use only when user specifies so.

**Instead:** Ask what the one thing this specific page needs the visitor to do or believe, and structure every element around that. Remove anything that does not contribute. Real IA is subtraction.

---

## Section 5 — Front-End Web Development (Web Developer perspective)

These are the patterns that a 40-year front-end engineer would call out in a code review.

### 5a. HTML defaults

- **Entire layouts built from `<div>` and `<span>`** with no semantic HTML — no `<main>`, `<nav>`, `<header>`, `<footer>`, `<article>`, `<section>`, `<aside>`, `<figure>`. Semantic HTML is not a nicety; it is the document model.
- **`<br><br>` used as a paragraph separator** instead of `<p>` elements with appropriate margin.
- **Inline `style` attributes** scattered through markup instead of class-based styling.
- **Images without `width` and `height` attributes** causing layout shift (Cumulative Layout Shift, CLS) as they load.
- **Missing `<meta name="description">`, `<meta property="og:title">`, `<link rel="canonical">`** — the minimum viable SEO and social-sharing metadata, absent.
- **`<title>` tags left as the framework default** — "React App," "Vite App," "My Next.js Project" — shipped to production.
- **No `lang` attribute on `<html>`** — preventing screen readers from using the correct language profile.
- **Non-descriptive link text** — "click here," "read more," "learn more" — instead of text that describes the destination.

### 5b. CSS defaults

- **`transition: all 0.3s ease` on every interactive element** — a single easing function and a single duration applied to every motion in the interface. Real motion design varies easing and duration based on the element's size, travel distance, and semantic weight.
- **`!important` used to override specificity conflicts** instead of fixing the underlying specificity problem.
- **Magic numbers in CSS** — `margin-top: 37px`, `padding: 13px 22px` — values with no relationship to a spacing scale.
- **No CSS custom properties (variables) for color, spacing, or typography** — values repeated literally across hundreds of lines.
- **`px` units for all font sizes and line heights** instead of `rem`/`em` — preventing the user's browser font-size preference from taking effect.
- **`z-index: 9999`** (or 999, or 99999) used as a blunt instrument without a defined stacking context strategy.
- **Media queries defined at arbitrary breakpoints** (768px, 1024px because those "feel like" tablet and desktop) rather than at the natural breakpoints of the content.
- **No `max-width` on body text** — lines of prose that stretch to 1400px on wide monitors, making the text unreadable.
- **CSS Grid or Flexbox used for everything including cases where one or the other is wrong** — Flexbox for two-dimensional grid layouts; Grid for single-axis flow.

### 5c. JavaScript defaults

- **`console.log` statements left in production code.**
- **Event listeners attached directly to DOM nodes inside loops** without delegation, creating memory leaks.
- **Fetching data without error handling** — `fetch(url).then(r => r.json()).then(setData)` with no `.catch()` and no loading/error state.
- **`useEffect` with an empty dependency array `[]` used as a componentDidMount substitute** in React, when the actual effect has dependencies that are not declared.
- **State stored in component local state that should be lifted**, causing prop-drilling ten components deep.
- **Entire feature flags implemented as `if (process.env.NODE_ENV === 'development')`** — not real feature flagging; just environment gating.
- **`any` type used everywhere in TypeScript** because adding types "takes too long" — defeating the purpose of using TypeScript at all.
- **No input sanitization** on user-supplied content before it is rendered into the DOM — XSS vulnerability introduced by default.
- **`setTimeout` used as a substitute for a proper loading state or event listener** — `setTimeout(() => setLoaded(true), 500)` as a hack that fails on slow connections.

### 5d. Performance defaults

- **Unoptimized images** — full-resolution PNGs or JPEGs served at display size, no WebP, no `srcset`, no `loading="lazy"` on below-fold images.
- **Loading all JavaScript in a single bundle** — no code splitting, no dynamic imports, no route-based chunking.
- **Third-party scripts loaded synchronously in `<head>`** — Google Analytics, chat widgets, A/B testing scripts blocking the main thread before the page renders.
- **No `font-display: swap`** on web fonts — invisible text during font load (FOIT) instead of a flash of system text (FOUT).
- **Render-blocking CSS** loaded via `<link rel="stylesheet">` for styles that are not used above the fold.
- **Web fonts loaded for weights and styles never used** — loading all 18 weights of a variable font "just in case."
- **Testing** - dont add scratch js, ts, or any other files in the code. Make sure the code is clean and well-organized.if added to check files, remove them.


**Instead:** Before writing a component or page, name the semantic elements that belong in it, the data flow, the error states, and the loading state. If you cannot name those, the component is not ready to be built.




---

## Section 6 — DevOps & Platform Engineering perspective

These are the patterns that a 40-year systems engineer or SRE would flag in an infrastructure review.

### 6a. CI/CD pipeline defaults

- **Three-stage pipelines (build → test → deploy) applied to every project** regardless of whether the project has tests, multiple deployment targets, or any deployment strategy beyond "push to main."
- **Hardcoded secrets in pipeline YAML files** — `API_KEY: "abc123"` directly in the workflow definition, not referenced from a secrets store.
- **`on: push` triggering pipelines on every branch** including branches that are not intended for deployment — no branch filtering, no path filtering.
- **No pipeline caching** for `node_modules`, dependency layers, or build artifacts — re-downloading the entire dependency graph on every run.
- **`npm install` instead of `npm ci`** in CI environments — non-deterministic installs that may differ from local development.
- **Deploying immediately on merge to main** with no staging environment, no smoke test, no deployment gate.
- **Health checks that only check HTTP 200** — not verifying that the application is actually serving correct content or that downstream dependencies are reachable.

### 6b. Docker and containerization defaults

- **`FROM node:latest`** (or any `latest` tag) — non-deterministic builds that break silently when the upstream image is updated.
- **Running containers as root** — no `USER` instruction in the Dockerfile, not `USER node` or a named non-root user.
- **Copying the entire project directory into the container** with `COPY . .` before installing dependencies — busting the Docker layer cache on every source change, including changes that do not affect dependencies.
- **No `.dockerignore` file** — copying `node_modules`, `.git`, test files, and local environment files into the image.
- **Multi-gigabyte images** because a full development environment (compilers, dev tools, test runners) was included in the production image instead of using a multi-stage build.
- **No `HEALTHCHECK` instruction** — the container reports healthy immediately on start regardless of whether the application inside it is actually ready.

### 6c. Infrastructure-as-code defaults

- **Hardcoded environment names, resource sizes, and region names** in Terraform or CloudFormation without variables or parameterization — impossible to reuse across environments.
- **No remote state backend** — Terraform state stored locally, making collaborative infrastructure management impossible.
- **`terraform apply` without `terraform plan` review** in an automated pipeline — applying infrastructure changes without a human-readable diff.
- **All infrastructure in a single monolithic file** — `main.tf` with 2,000 lines covering networking, compute, databases, and IAM in one place.
- **No tagging strategy** for cloud resources — impossible to attribute costs, identify owners, or implement resource lifecycle policies.
- **Wide-open security groups** — `0.0.0.0/0` on ingress rules for ports that should only be accessible from a VPC or a specific IP range.
- **No log retention policy** — logs accumulating indefinitely in a storage bucket or log group with no expiration.

### 6d. Monitoring and observability defaults

- **No structured logging** — `console.log("something happened")` strings with no timestamp, no request ID, no severity level, no machine-parseable format.
- **Alerts only on downtime** — no alerting on latency percentiles (p95, p99), error rate thresholds, or saturation signals.
- **Dashboards with 30 panels covering every metric** without a clear answer to: what does "healthy" look like on this dashboard, and what does "failing" look like?
- **No runbook linked from alerts** — an on-call engineer receives a page with no documented procedure for investigating or remediating the issue.
- **Single-environment monitoring** — production is monitored but staging is not, meaning regressions are only caught in production.

**Instead:** For every piece of infrastructure or pipeline code generated, state what the production environment, team size, and deployment frequency are. If those are unknown, say so rather than generating a generic three-stage YAML and calling it production-ready.

---

## Section 7 — Content Development & Documentation (Technical Writer / Content Strategist perspective)

### 7a. Documentation defaults

- **README files that describe what the project is without explaining how to use it** — paragraphs of feature description, followed by a badge row, followed by a one-line installation command and nothing else.
- **Installation instructions that assume a clean machine** — no mention of required Node version, Python version, system dependencies, or environment variable configuration.
- **No "Getting Started" path** distinct from "Full API Reference" — every user, whether beginner or expert, is dumped into the same flat documentation structure.
- **Code examples with no error paths shown** — only the happy path, never the "what do I do if this returns a 401" path.
- **Changelog entries that say "Bug fixes and performance improvements"** with no specifics — copied from Apple's iOS release notes, equally uninformative.
- **API documentation that only documents parameters** without explaining when to use the endpoint, what preconditions must be true, and what the caller is responsible for after calling it.
- **Outdated screenshots in documentation** — showing a UI that no longer exists, eroding trust in every other document in the system.

### 7b. Content strategy defaults

- **Publishing cadence set to "2 posts per week"** without any analysis of whether this audience reads that much, whether there is enough original material to sustain it, or whether the posts will have any distribution.
- **Topic selection by keyword volume alone** — writing about whatever has the highest search volume rather than what the product team has genuine expertise or opinion about.
- **"Pillar page" and "cluster content" architectures** generated as the default SEO content strategy without knowing whether the product's buyers use search at all.
- **Case studies that describe what was done but not what the outcome was** — "We helped Company X redesign their dashboard" with no before/after metric.
- **Video transcripts auto-published as blog posts** with no editing — the grammar of spoken word is different from the grammar of written prose; they are not interchangeable.

---

## Section 8 — Cross-Discipline Code Quality (All Engineering roles)

These are failures that cut across every technical discipline.

- **God components / god functions** — a single React component or function that handles data fetching, business logic, formatting, error handling, and rendering. Every discipline's equivalent of the "one big file."
- **No error boundaries** in React trees — a single component failure brings down the entire UI subtree with a white screen.
- **No environment variable validation on startup** — the application starts, runs fine until it tries to use a missing API key 10 minutes later, and fails with a cryptic error that has nothing to do with the root cause.
- **`git commit -m "fix"` or `git commit -m "update"` as commit messages** — no context, no scope, no ability to understand what changed from the history.
- **Dependencies pinned to `^major.minor.patch`** in `package.json` — allowing minor and patch updates automatically, meaning the same `npm install` produces different results six months later.
- **No `.nvmrc` or `engines` field in `package.json`** — the required Node version is documented nowhere, and the project silently fails on older or newer runtimes.
- **Tests that only test the happy path** and are designed to pass, not to catch regressions.
- **Copy-pasted code across three files** with slight variations instead of an abstracted, parameterized function — three bugs introduced simultaneously when the logic needs to change.
- **Over-engineered abstractions for a project that is not yet large enough to need them** — microservices for a solo-developer project, a design system for a four-page site, event sourcing for a to-do list.

---

## Section 9 — The Final Self-Check (Every Discipline)

Before showing any output — visual, copy, structural, or technical — answer these questions. If any answer is "no" or "I don't know," revise before showing.

1. **Is this output specific to this product, team, or context?** Could the code, copy, or design be lifted verbatim into a different product and still read as correct? If yes, it is generic. Revise.

2. **Did I choose this because it is right, or because it was the first thing that came to mind?** The first-instinct output of a language model is, by definition, the statistical average of its training distribution. The average is not the premium. The average is the slop.

3. **Is there a concrete, specific fact driving this choice?** A real measurement, a named constraint, a specific user need, an actual business rule — not a vibe, not "it looked tech-company enough."

4. **Would a 40-year practitioner in this discipline be embarrassed to ship this?** The senior engineer who has written more bad code than you have written any code can spot these patterns in seconds. Would they call a code review? Would they red-pen the copy? Would they reject the design in critique?

5. **Have I said what this is NOT going to do?** Real professional output includes constraints, edge cases, and explicit non-goals. Slop only describes the happy path.

6. **Is there anything in this output that exists only because I thought it was expected, not because it serves the user?** The third pricing tier. The FAQ section. The "About Us" page. The dark mode. The particle background. If you cannot name why it is there, remove it.

---

## Section 10 — How to Respond When Pushed Back

If the user says "this still looks AI-generated," "this is generic slop," "this looks like every other SaaS site," or "a junior could have written this":

**Do not:** Adjust spacing. Change the color. Swap one icon for another. Add more sections. Make the font bigger.

**Do:** Name the specific item from the checklist above that you defaulted to. State it explicitly: "I defaulted to [pattern]. The replacement decision is [specific, justified alternative]." Then rebuild from that replacement decision, not from the previous draft with surface changes applied.

The difference between a 40-year practitioner and a model generating defaults is not technique — it is the willingness to throw away a draft that has no specific reason to exist.

---

## Section 11 — Source Code / "View Source" Tells

Right-click → View Page Source (Ctrl+U on Windows, Cmd+Option+U on Mac) to see the raw HTML. Look for:

- **AI-authored comments left in.** Some developers leave comments in the code explicitly marking sections as AI-generated — rare, but an instant confirmation when present.
- **Over-engineered structure for trivial functionality.** A vibe-coded script that does something simple may still include a full repository pattern, abstract base classes, dependency injection, and factory methods — all for ten lines of actual logic. Human developers calibrate complexity to the size of the problem.
- **Inconsistent patterns across the same site.** Authentication might use one pattern in one module and a completely different pattern in another, with no coherent reason — a sign of separate prompts/sessions making independent decisions with no unifying architecture.
- **Bloated dependency list.** A vibe-coded project may pull in 80+ dependencies for a simple web app — each one a library the model reached for reflexively rather than using a stdlib equivalent.
- **Builder/tool fingerprints in the JS bundle.** Even when a site is on a custom domain with builder branding removed, scanning the JavaScript bundle can reveal Lovable artifact strings, v0 component patterns, or Bolt runtime identifiers that survive de-branding.
- **The "default AI stack."** Next.js + Tailwind CSS + Shadcn UI + Lucide Icons + Radix UI is the component stack AI coding tools reach for by default — not proof on its own (plenty of humans choose this stack deliberately), but raises the prior when combined with other signals.
- **Meta tag oddities.** Strange spellings or generic phrasing in meta tags can indicate an AI tool generated them, even if the visible page content was human-written.

---

## Section 12 — Technical / Performance Tells

- **Slower-than-expected load times.** AI-generated code is often heavier than necessary, which drags down Core Web Vitals scores — check via Chrome DevTools → Lighthouse, or PageSpeed Insights.
- **Accessibility gaps.** Missing alt text, unlabeled buttons, and poor keyboard navigation support are common when no human reviewed the output.
- **Missing SEO/AEO basics.** No meta descriptions, no Open Graph images, duplicate page titles, no structured data, and a thin or skipped heading hierarchy all suggest a site that shipped without an SEO pass.
- **No real backend signal.** A site with form fields that don't actually submit anywhere, or a "Sign up" flow that goes nowhere — common when a UI was generated without a working backend behind it yet.

---

## Section 13 — Strategic / Business-Context Tells (The Deepest Signal, Hardest to Fake)

This is the layer pure code-scanning tools can't see, and arguably the most reliable:

- **No clear job the site is doing.** The site looks like a website but isn't built to do anything specific — book calls, generate leads, qualify prospects — it's just present.
- **No conversion thinking.** Page structure, user journey, and calls to action feel like an afterthought rather than a designed path.
- **Positioning vacuum.** The site never clearly states who it's for or why someone should pick it over alternatives — because the model was never given that strategic context to begin with, only a feature list to describe.


## Section 14 - Deploying code / Upoading to Git 

- **Dont commit**- Dont use git init or git add or git commit . Also dont add any scratch files to the repo. Make sure the code is clean and well-organized.Let the user do this.  