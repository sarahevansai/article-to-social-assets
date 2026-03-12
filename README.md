# Article → Social Assets

Convert any article into 5 professional, branded social media promotion images in minutes.

## What It Does

Share an article URL + pull quote + branding source → get:

- **LinkedIn hero** (1200×630) — professional layout with quote, logo, branding
- **X/Twitter card** (1024×512) — compact optimized for Twitter
- **Instagram Story 1** (1080×1920) — quote feature with branding
- **Instagram Story 2** (1080×1920) — key insights breakdown
- **Instagram Story 3** (1080×1920) — call-to-action & full article link

All images include:
- ✅ Your actual logo/branding
- ✅ Professional typography & layout
- ✅ Dark professional theme
- ✅ Safe zones for mobile viewing
- ✅ Clear attribution & CTA

## Use Cases

- **Thought leadership articles** — promote your own or guest posts
- **Press releases** — turn announcements into shareable assets
- **Interviews** — feature yourself or your team being quoted
- **Case studies** — showcase client wins
- **News mentions** — amplify earned media coverage
- **Industry insights** — share reports, research, whitepapers

Works with **any article format** — news, blog posts, interviews, announcements, research papers.

## Installation

### Via OpenClaw Workspace

Clone directly into your skills folder:

```bash
git clone https://github.com/sarahevansai/article-to-social-assets.git ~/.openclaw/workspace/skills/article-to-social-assets
```

### Via ClawHub (when published)

```bash
clawhub install article-to-social-assets
```

## Usage

When you have an article to promote, trigger the skill:

```
I want to promote this article: [paste article URL]

Pull quote: "Your direct quote from the article"

Branding source: [paste URL where we should pull your logo/colors]
```

### Example Inputs

**Article URL:**
```
https://www.odwyerpr.com/story/public/24430/2026-03-10/how-brands-can-stay-visible-age-ai.html
```

**Pull Quote:**
```
"What's next is just an understanding of AI visibility and how your brand is being interpreted by AI"
```

**Branding Source:**
```
https://linkedin.com/company/zen-media (or https://yourcompany.com)
```

## Output

The skill generates:
- 5 high-quality PNG files, all platform-optimized
- HTML preview showing all 5 images together
- Download links ready to share
- Files saved to `/projects/social-assets/[article-slug]/`

## How It Works

1. **Fetches article content** — extracts title, description, publication, author
2. **Pulls branding** — visits your provided URL to grab logo & colors
3. **Designs assets** — uses AI to create professional layouts with your quote
4. **Exports images** — PNG format, ready to upload directly to each platform
5. **Delivers to you** — Telegram notification with preview & download links

## Requirements

- Active OpenClaw instance
- Google Workspace access (for article fetching)
- Branding source URL (company site, LinkedIn profile, etc.)
- A pull quote from the article (copy-paste)

## Platform Specs (Included)

- **LinkedIn:** 1200×630px, optimized for feed
- **X/Twitter:** 1024×512px, optimized for cards
- **Instagram Stories:** 1080×1920px (3 variants), safe zones respected

## Examples

See the `references/workflow.md` for detailed workflow documentation.

## Support

Questions or issues? Check the skill's workflow reference or adjust branding URL if logo isn't detected.

## License

MIT License — free to use and modify for personal and commercial use.

---

Built with ❤️ by Sarah Evans (asksarah.ai)
