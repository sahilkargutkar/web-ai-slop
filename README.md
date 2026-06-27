# Web AI Developer Toolkit

[![skills.sh](https://skills.sh/b/sahilkargutkar/web-ai-slop)](https://skills.sh/sahilkargutkar/web-ai-slop)

A suite of Agent Skills designed to improve web development and copywriting when working with AI coding assistants (like Cursor, Claude Code, and Windsurf). 

This toolkit contains two complementary skills:
1. **`web-ai-slop` (The Anti-Default Filter)**: Catch and eliminate generic AI design patterns, visual clichés, copywriting tropes, and code tells before shipping.
2. **`aeo-geo-writing` (The AI Citation Structurer)**: Optimize and format web copy to be retrieved, cited, and attributed by generative search engines (ChatGPT, Perplexity, Gemini, Google AI Overviews, and Claude).

---

## Installation

Install these skills into your AI agent workspace using the `skills` CLI:

### Install Both Skills (Recommended)
```bash
npx skills add sahilkargutkar/web-ai-slop --all
```

### Install a Specific Skill
To add only the Anti-Default Filter:
```bash
npx skills add sahilkargutkar/web-ai-slop --skill web-ai-slop
```

To add only the AI Citation Structurer:
```bash
npx skills add sahilkargutkar/web-ai-slop --skill aeo-geo-writing
```

To preview either skill locally without installing:
```bash
npx skills use ./@web-ai-slop --skill web-ai-slop
# or
npx skills use ./@web-ai-slop --skill aeo-geo-writing
```

---

## The Skills

### 1. Web AI Slop (`skills/web-ai-slop`)

Large language models converge on the same "safe" statistical defaults when generating websites. This skill acts as a gatekeeper, prompting your agent to discard generic drafts and make intentional design decisions.

*   **Visual Clichés**: Glowing gradient blobs, particle networks, glassmorphism cards, excessive border-radius, pill CTAs, bento grids, and Shadcn default styles.
*   **Color & Type Defaults**: Standard purple-to-blue palettes, unadjusted letter-spacing on display headings, and default Inter font stacks.
*   **Copywriting Clichés**: Vague SaaS empowerment verbs (*supercharge*, *empower*, *elevate*, *unlock*), rule-of-three adjective stacks (*Fast. Secure. Reliable.*), and throat-clearing openings.
*   **Dev & UX Tells**: Monolithic section flows, placeholder image services, 3-tier pricing sections with fake recommended highlights, and `transition: all 0.3s ease` on everything.

*How it works*: When the agent runs a draft against the checklist and finds **2 or more matches** in any category, it flags it as slop. The agent is forced to discard the draft and write a unique solution.

### 2. AEO/GEO Copywriting (`skills/aeo-geo-writing`)

AI search engines (RAG) do not read websites like humans or index pages like traditional SEO. They retrieve standalone text chunks and analyze them for authority, freshness, and attribution. This skill optimizes your content to be cited by name by LLM systems.

*   **Answer Capsules**: 40–60 word declarative summaries directly beneath H2 headings, containing no preamble or fluff.
*   **Authority & Citability**: Eliminates hedging (*we believe*, *probably*), replaces adjectives with checkable numbers/metrics, and names reliable sources directly.
*   **Extraction Semantics**: Uses HTML `<table>` elements for comparisons, embeds `FAQPage` schema on interactive questions, and places an `llms.txt` file at the domain root.
*   **Platform Tuning**: Tailors copy structure for the specific biases of ChatGPT (verbatim definitions), Perplexity (freshness/data), Google AI Overviews (rich schema), and Claude (reasoning depth).

---

## Detection & Auditing

*   Want to audit an existing website to see if it was built by AI? Check out **[docs/detecting-ai-slop.md](docs/detecting-ai-slop.md)** — a comprehensive inspection guide for visual, copywriting, UX, code, and DevOps tells, including a scoring rubric.
*   Try the interactive web scanner and AEO copy grader online at [https://sahilkargutkar.github.io/web-ai-slop/](https://sahilkargutkar.github.io/web-ai-slop/).

---

## Contributing

If you spot new AI default patterns or discover better generative citation techniques, please open a Pull Request!
- Update `skills/web-ai-slop/SKILL.md` to add new anti-slop checks.
- Update `skills/aeo-geo-writing/SKILL.md` to improve generative search guidelines.
- Modify `docs/detecting-ai-slop.md` to update the website inspection guide.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
