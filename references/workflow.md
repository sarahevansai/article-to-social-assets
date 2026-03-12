# Article → Social Assets Workflow

## Input Collection

Ask user for:
1. **Article URL** — what are they promoting?
2. **Quote** — what's the key statement to highlight?
3. **Branding URL** — where to pull logo/colors from?

## Processing Pipeline

### Step 1: Fetch Article
- Use web_fetch to pull article content
- Extract: title, description, author, publication, key images
- Parse metadata (byline, date, publication name)

### Step 2: Extract Branding
- Visit provided branding URL
- Pull: company logo (PNG/SVG preferred)
- Detect: primary brand colors (from logo or website)
- Fallback: dark professional theme (blues/oranges) if colors unclear

### Step 3: Generate Assets
Use Sonnet to create 5 images:
1. **LinkedIn hero** (1200×630)
   - Publication logo top-left
   - Article title headline
   - Large user photo (if available from article/profile)
   - Pull quote in prominent text box
   - Attribution + CTA
   - Branding footer

2. **X card** (1024×512)
   - Compact layout
   - User photo + handle
   - Publication logo
   - Headline + quote excerpt
   - Branding footer

3. **Instagram Story 1** (1080×1920)
   - Publication logo
   - Pull quote (full) as primary visual
   - Article headline
   - User mention
   - Branding footer

4. **Instagram Story 2** (1080×1920)
   - 3-5 key insights/callouts from article
   - Numbered cards or breaking points
   - User branding
   - Footer CTA

5. **Instagram Story 3** (1080×1920)
   - User photo if available
   - "Full article" headline
   - Link to original article
   - Branding/hashtag footer

### Step 4: Save & Output
- Save all 5 images to `/projects/social-assets/[article-slug]/`
- Create HTML preview showing all 5 together
- Provide download links
- Confirm file sizes and dimensions

## Technical Notes

**Image Generation:**
- Use Sonnet via sessions_spawn for image layout/design
- Leverage web_fetch for pulling external assets
- Image tool for analyzing branding colors

**File Naming:**
- `linkedin-[article-slug]-final.png`
- `twitter-[article-slug]-final.png`
- `instagram-story-1-[article-slug]-final.png`
- `instagram-story-2-[article-slug]-final.png`
- `instagram-story-3-[article-slug]-final.png`

**Quality Checks:**
- Verify all images meet platform specs (dimensions, safe zones)
- Check text readability on mobile/light modes
- Confirm branding is visible and professional
