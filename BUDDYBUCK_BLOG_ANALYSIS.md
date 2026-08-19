# BuddyBuck.com Blog Analysis

**Analyzed:** August 19, 2026
**Pages scraped:** Homepage, blog index, 4 individual posts (Wallaby Story, Milk Aisle Meeting, $250K Over Asking, Duvall neighborhood guide)
**Purpose:** Model the blog structure, voice, and SEO approach for YNSH blog posts

---

## Site Architecture

- **Platform:** Next.js on Vercel (buddybuck-next.vercel.app)
- **URL structure:** /blog/[keyword-rich-slug] (clean, no .html extension)
- **Blog index:** /blog with card-style listing (all posts, no pagination visible)
- **Content volume:** 26+ blog posts as of August 2026
- **Categories used:** Client Stories, Personal Branding, Local Expertise, Business Philosophy, Case Studies, Neighborhood Guide, Schools & Education, Buyer Education, Market Analysis, Lifestyle

## Blog Post Structure (Individual Posts)

### Layout Elements
1. **Back to Blog** link at top
2. **Category label** (e.g., "Client Stories", "Neighborhood Guide")
3. **H1 title** (geographic keywords embedded)
4. **Metadata line:** Date, read time, "By Buddy Buck, eXp Realty, Duvall, WA"
5. **Hero image** (full-width, high quality)
6. **Body content** with H2 subheadings
7. **Author bio card** at bottom (name, brokerage, stats, phone)
8. **CTA section:** "Ready To Write Your Duvall Story?" with booking link
9. **"More Stories" section:** 3 related posts as cards

### Content Patterns

**Deal Stories (Client Stories / Case Studies):**
- Narrative arc: Situation, Challenge, How Handled, Outcome
- First-person voice throughout ("I said," "My answer was")
- Specific numbers: dollar amounts, timelines, percentages
- Named vendor partners (contractor, stager, videographer)
- Client quotes used as pull quotes
- Takeaway/lesson section at the end
- Strong hooks in opening paragraphs (anecdotes, not stats)
- Word count: 800-1,200 words for stories, 1,500+ for full case studies

**Neighborhood Guides:**
- Lead with surprising data point or comparison
- "The Numbers" section with median prices, commute times, comparisons to neighboring areas
- "The Community Factor" section with local color, events, personality
- "Who Buys Here" buyer profile section
- "The Bottom Line" honest assessment (what's great AND what's not)
- Word count: 800-1,200 words
- Conversational, opinionated, not generic chamber-of-commerce copy

## SEO / AEO Strategy

### Meta Tags
- `meta-author`: Agent name
- `meta-description`: Keyword-rich, 150-160 chars, includes city + deal type
- `meta-og:type`: "article" for blog posts
- `meta-robots`: "index, follow"
- `meta-googlebot`: "index, follow, max-video-preview:-1, max-image-preview:large, max-snippet:-1"
- Canonical URL set
- Full Open Graph and Twitter Card tags

### Keyword Placement
- Geographic keywords in: title tag, H1, meta description, OG title/description, body H2s
- City name appears in slug (e.g., /bellevue-inheritance, /duvall-best-kept-secret)
- Comparative keywords used to capture cross-market searches ("Snoqualmie Ridge vs. Issaquah Highlands")
- Long-tail question format absent from H2s (Buddy uses statement H2s, not questions)

### Schema Markup
- No visible JSON-LD in the fetched HTML (likely injected via Next.js Head component)
- Article meta tags present (og:type = article)
- Author attribution consistent

## Blog Index Card Format

Each card on /blog contains:
- Category tag (colored label)
- Read time ("5 min read")
- Title (clickable, linked)
- Summary (1-2 sentences)
- Date (Month Day, Year format)
- "Read more" link

## Visual Layout

- Clean, minimal design with generous white space
- Full-width hero images on individual posts
- No visible Google Maps embeds in blog posts
- No visible photo galleries or slideshows in posts
- Author photo in bio card
- Consistent typography (likely Inter or similar sans-serif)

## Photo Handling

- Hero images per post (property shots or location shots)
- Next.js Image optimization (/\_next/image?url=...&w=3840&q=75)
- Alt text describes the post topic, not the image content
- Testimonial section uses client photos
- No inline images within post body (text-only body content)

## What to Adapt for YNSH

### Keep from Buddy Buck:
1. Strong narrative arc for deal stories (Situation, Challenge, Solution, Outcome)
2. First-person voice throughout
3. Specific numbers (prices, timelines, percentages)
4. Honest "bottom line" sections in neighborhood guides
5. Author bio card with credentials + CTA
6. Category labels and read time estimates
7. Related posts section at bottom
8. Keyword-rich slugs

### Change for YNSH:
1. **Use question-format H2s** for AEO (Buddy uses statements; Becca should use questions per existing KEYWORD-STRATEGY.md)
2. **Add JSON-LD** (Article + LocalBusiness structured data)
3. **Add Google Maps embed placeholders** (Buddy doesn't embed maps; YNSH should for local SEO)
4. **Pierce County geography** instead of Snoqualmie Valley
5. **Becca's voice** (warmer, funnier, more self-deprecating than Buddy's confident/assertive tone)
6. **Solo agent framing** (I/me, no team references beyond TC/vendors)
7. **Photo placeholders** for both listing photos and neighborhood photos per Brett's dual-photo strategy
8. **Fair housing compliance filter** on all neighborhood descriptions
9. **Static HTML format** matching existing YNSH site design (not Next.js)

### Content Cadence (Buddy's Model):
- Mix of deal stories (3-4 per quarter) and neighborhood guides (1-2 per month)
- Backdated posts to establish content depth
- Seasonal/topical posts sprinkled in
- Every post ends with a clear CTA

---

*This analysis informs the first batch of 5 YNSH blog posts.*
