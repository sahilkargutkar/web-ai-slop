# Web AI Slop

[![skills.sh](https://skills.sh/b/sahilkargutkar/web-ai-slop)](https://skills.sh/sahilkargutkar/web-ai-slop)

An Agent Skill to filter out generic AI-generated design patterns, visual clichés, copywriting tropes, and code tells before shipping. 

This skill acts as a deliberate filter. Rather than enforcing a single visual style, it identifies the statistical "safe" averages that large language models default to when generating websites, landing pages, marketing copy, or application interfaces, prompting the agent to step away from them and make intentional design choices.

---

## Installation

Install this skill into your AI agent workspace (e.g., Claude Code, Cursor, Windsurf) using the `skills` CLI:

```bash
npx skills add sahilkargutkar/web-ai-slop
```

To run or preview the skill locally without installing:

```bash
npx skills use ./@web-ai-slop
```

---

## How It Works

Before your AI agent generates a layout, designs a component, or drafts copy, it runs its plan against the check categories. If the proposed output matches **2 or more** items in any category, it is flagged as a default average (slop). The agent is instructed to discard the draft and make a specific, localized design decision.

### Categories Tracked

1. **Visual Clichés**: Aurora/gradient background blobs, floating dot/particle networks, bento grids of Lucide icons, glassmorphism cards with white borders, glowing brand shadows, and dashboard widget wallpapers.
2. **Color & Type Defaults**: Default purple-to-blue palettes, unadjusted letter-spacing on display headlines, absence of visual type hierarchy, and lack of display face considerations.
3. **Copywriting Clichés**: Vague SaaS verbs ("unlock," "elevate," "supercharge"), rule-of-three adjective stacks ("Simple. Powerful. Secure."), throat-clearing openings, and em-dash-heavy declarations.
4. **Structural/UX Defaults**: Rigid, formulaic section sequences (Hero → Logos → Bento Features → Testimonial Carousel → 3-Tier Pricing → FAQ → CTA → Footer), default 3-tier pricing highlighting the middle card without product justification, and stock testimonials.
5. **Code tells**: Unremoved lorem ipsum, placeholder image services (e.g. `placeholder.com`), comment scaffoldings, and single-easing transitions (`all 0.3s ease`) applied to all elements.

---

## Contributing

If you find a new pattern that AI models constantly default to when generating web applications, feel free to open a Pull Request updating `SKILL.md`.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
