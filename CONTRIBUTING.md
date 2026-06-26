# Contributing to Web AI Slop

Thank you for your interest in contributing to Web AI Slop! We want to help creators, designers, and developers filter out statistical, unoriginal AI-generated defaults to encourage intentional, human-centered design.

By contributing, you help make the AI web cleaner, more diverse, and more thoughtful.

---

## What We Are Looking For

We welcome contributions of all kinds, but we are specifically looking for additions to our "Tells" and "Clichés" lists in:
1. **[skills/web-ai-slop/SKILL.md](skills/web-ai-slop/SKILL.md)** — The direct agent prompt instructions.
2. **[docs/detecting-ai-slop.md](docs/detecting-ai-slop.md)** — The audit checklist guide.

### Criteria for a Tell or Cliché
Before proposing a new item, ask yourself:
* **Is it a statistical average?** Does it default to this across multiple models (e.g., Claude, ChatGPT, Gemini, v0) because of training data bias?
* **Is it a shortcut?** Does it represent a lack of intentional design decisions (like using `transition: all 0.3s ease` on every single element to make it "animated")?
* **Is it distinct from style?** Avoid targeting specific design styles simply because you dislike them. The goal is to flag *unreviewed defaults*, not restrict aesthetic diversity.

---

## Local Setup & Development

To test and preview the skill locally:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sahilkargutkar/web-ai-slop.git
   cd web-ai-slop
   ```

2. **Test/Preview the Skill:**
   You can run the skill locally in your terminal or an AI agent workspace using:
   ```bash
   npx skills use .
   ```
   Or if using a global installation:
   ```bash
   npx skills use ./skills/web-ai-slop
   ```

---

## How to Propose Changes

### Step 1: Check Existing Work
Search the open issues and pull requests to ensure someone else hasn't already proposed or implemented the same change.

### Step 2: Create a Branch
Create a new branch for your changes:
```bash
git checkout -b feature/add-new-tell-category
```

### Step 3: Make Your Changes
Modify the appropriate files. Be specific, clear, and provide context:
* **For `skills/web-ai-slop/SKILL.md`**: Keep it brief and instructions-oriented.
* **For `docs/detecting-ai-slop.md`**: Provide an explanation, a checklist checkbox, and maybe why it represents a default tell.

### Step 4: Commit and Push
Commit your changes with clear, descriptive commit messages:
```bash
git commit -m "docs: add aurora background gradient tell to visual clichés"
git push origin feature/add-new-tell-category
```

### Step 5: Open a Pull Request
Open a pull request on GitHub. Fill out the pull request template so we can review it promptly.

---

## Code of Conduct

This project is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to the project maintainers.
