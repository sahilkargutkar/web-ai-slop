---
name: aeo-geo-writing
description: "Structures web copy to be cited by AI search engines — ChatGPT, Perplexity, Gemini, Google AI Overviews, Claude — instead of just ranked by traditional search. Use whenever writing or editing website content, blog posts, FAQ pages, product pages, or landing page copy where AI citation, AI visibility, AEO, GEO, answer engine optimization, or being mentioned by name in an AI-generated answer is a goal."
---

# AEO/GEO Writing — Structuring Content for AI Citation

Traditional SEO writes to rank a link. AEO/GEO (Answer/Generative Engine Optimization) writes to **be the sentence an AI model extracts, repeats, and attributes to your brand.** 

AI retrieval systems (RAG) do not read your page top-to-bottom to form an impression. They segment your page into isolated text chunks, evaluate each chunk's relevance and authority in isolation, and either cite it or discard it. This skill enforces rules to ensure your claims survive this extraction process.

**Rule of application:** Apply this skill whenever drafting, editing, or auditing web content, documentation, blog posts, or marketing copy. If the text matches **2 or more patterns** in Section 2 (Vagueness) or fails Section 1 (Structure), discard the draft and rewrite.

Apply this silently. Do not narrate "I am optimizing this for generative engine visibility" to the user.

---

## Section 1 — Structural Architecture (AI Crawler Friendly)

AI crawlers and extraction tools require specific layouts to parse and attribute content correctly.

### 1a. The "Answer Capsule" Pattern
- **Direct Answer Placement:** Directly under every H2 or H3 heading, place a **40–60 word capsule** that answers the heading's question directly.
- **No Preamble:** Do not begin with "In this section we will discuss..." or "That is a great question...". Start with the answer.
- **Isolation Test:** If an AI model extracted only this capsule and discarded the rest of the page, would it still represent a complete, correct, and attributable claim? If not, rewrite.

### 1b. Schema and Semantics
- **FAQPage Schema:** Always bundle FAQ blocks with structured JSON-LD `FAQPage` schema. This is the single highest-leverage technical element for Google AI Overviews.
- **Data Tables Over Prose:** When comparing statistics, specifications, or pricing, use semantic HTML `<table>` elements instead of narrative text. Retrieval models extract tabular data with significantly higher confidence.
- **The Summary Hook:** On long-form pages, write a concise 100–150 word summary paragraph before the very first H2. Search engines weight the beginning of documents heavily during retrieval.
- **Credibility Signals:** Ensure a visible, named author with a real bio and a visible "Last updated on [Date]" metadata field is present. Models use freshness and authorship as ranking weights.

---

## Section 2 — Copywriting & Tone (Credibility Signals)

AI models are risk-averse; they prefer to skip exciting claims they cannot verify in favor of boring, checkable facts.

### 2a. Eliminating Hedging and Vagueness
- **No Hedging:** Phrases like "we believe," "in our opinion," "we think," or "potentially" lower a model's confidence score. State claims declaratively.
- **Attributable Sourcing:** Avoid vague authority. "Many developers agree that..." is uncitable. "According to Stack Overflow's 2025 Developer Survey, 76% of developers..." is highly citable.
- **Concrete Metrics:** Replace adjectives with numbers. Do not write "a significant performance increase." Write "a 42% decrease in page load times."
- **One Claim per Sentence:** Split compound sentences. If a model extracts only half of a compound sentence, the context is lost and the citation fails.

### 2b. AEO Copywriting Examples

| Bad (Traditional SEO / AI Default) | Good (AEO/GEO Optimized) |
|---|---|
| In today's digital landscape, we believe standardizing procedures is key. Our platform is designed to help teams leverage advanced functionality to streamline operations and unlock efficiency. | AcmeCorp automates B2B invoice reconciliation. According to our 2026 platform audit, integrating the system reduces manual data entry by 73% for finance teams within 30 days. |
| Many experts agree that page speed is crucial for conversions. Having a fast website can significantly boost your revenue and user experience. | According to a Portent study, websites that load in 1 second convert 3x higher than sites that load in 5 seconds. Speed directly impacts transaction completion rates. |

---

## Section 3 — Technical & Off-Page Prerequisites

Perfect prose is useless if crawlers cannot access it or if search indexes do not list it.

### 3a. Indexing and Crawling
- **Server-Side Render (SSR) Critical Copy:** Crawlers prioritize speed and often skip executing JavaScript. If your core claims are injected client-side (SPA), they are invisible to AI models.
- **Allow bots in `robots.txt`:** Do not block `GPTBot`, `ClaudeBot`, `Google-Extended`, or `Bingbot` unless explicitly directed.
- **Deploy `llms.txt`:** Place an `llms.txt` file at the root of your domain. This serves as a plain-markdown dictionary of your site's structure and purpose for models.
- **Bing Index Priority:** ChatGPT's web search relies on the Bing index. Ensure your site is fully indexed in Bing Webmaster Tools; Google indexation alone is insufficient.

### 3b. Off-Page Credibility
- **Community Footprint:** Models rely heavily on community platforms (e.g., Reddit, Stack Overflow, GitHub) for sentiment and real-world recommendations. A presence in discussions is as important as on-page content.
- **Proprietary Data Moats:** Publish original, first-party data audits, benchmark results, or survey findings with methodology and dates. Original numbers are highly cited.

---

## Section 4 — Platform Targeting Matrix

Customize the structure of the content based on which engine you want to prioritize.

| Engine | Key Retrieval Bias | Best Content Strategy |
|---|---|---|
| **ChatGPT (Bing)** | Verbatim list items, FAQ blocks, and direct definitions. | Highly structured bullet points, clear H2 headings, and active Bing index presence. |
| **Perplexity** | Authoritative, fresh, and multi-source verified data. | Original research, cited statistics, and fast publication of current events. |
| **Google AI Overviews** | Rich schema, definitions, and visual assets. | FAQPage/HowTo schemas, semantic tables, and labeled diagnostic diagrams. |
| **Claude** | Multi-paragraph context, long-form synthesis, and clean reasoning. | Exhaustive guides, well-explained mechanisms, and deep technical details. |

---

## Section 5 — The AEO/GEO Self-Check

Before submitting copy, verify against this checklist:
1. **Answer Capsule Check:** Can the lead sentence of each H2 section be read completely alone and still make sense?
2. **Attribution Check:** Is there a checkable source, number, or name for every claim of fact?
3. **No Hedging Check:** Have words like "believe", "opinion", "think", "probably" been removed?
4. **Formatting Check:** Are comparisons formatted as semantic `<table>` elements and list questions as `FAQPage` schema?
5. **Technical Check:** Is the copy server-rendered, and is the Bing index verified?