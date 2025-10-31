# Visual Enhancement Guide for Annoushka AI Hub

This guide shows you how to use brand assets to make the AI Hub more appealing for creatives.

## What We've Implemented

### 1. Custom Brand Fonts ✅
**Location**: `mint.json`

```json
"font": {
  "headings": {
    "family": "Masny",
    "weight": 600
  },
  "body": {
    "family": "Contane",
    "weight": 400
  }
}
```

**Fonts Available**:
- **Masny**: Light, Book, Regular, SemiBold (+ italics) - Used for headings
- **Contane**: Regular, Semibold, Text variants (+ italics) - Used for body text

**Location**: `public/brand guidelines/Annoushka_BRAND_fonts/`

---

### 2. Hero Images on Key Pages ✅

**Implementation Pattern**:
```mdx
<img
  src="/images/JPG_2025/LOOK_XX_XXX copy.jpg"
  alt="Descriptive alt text"
  style={{ width: '100%', borderRadius: '12px', marginBottom: '2rem', maxHeight: '350px', objectFit: 'cover' }}
/>
```

**Pages Enhanced**:
- ✅ Introduction page - `LOOK_07_127 copy.jpg`
- ✅ Marketing prompts - `LOOK_02_285 copy.jpg`
- ✅ Social Media prompts - `LOOK_09_269 copy.jpg`
- ✅ ChatGPT Projects guide - `LOOK_05_057 copy.jpg`

**Available Images**: 19 high-quality campaign photos in `public/images/JPG_2025/`

---

### 3. Image Galleries ✅

**Implementation on Social Media Page**:
```mdx
<CardGroup cols={3}>
  <Card>
    <img src="/images/JPG_2025/LOOK_01_156 copy.jpg" style={{ borderRadius: '8px' }} />
  </Card>
  <Card>
    <img src="/images/JPG_2025/LOOK_08_086 copy.jpg" style={{ borderRadius: '8px' }} />
  </Card>
  <Card>
    <img src="/images/JPG_2025/LOOK_12_051 copy.jpg" style={{ borderRadius: '8px' }} />
  </Card>
</CardGroup>

<Tip>
**Visual Inspiration**: Use these images as references when describing content to AI.
</Tip>
```

---

### 4. Loom Video Embeds (Templates Ready) ✅

**Current Status**: Video embed templates are already in place, just need recording!

**How to Add Your Loom Video**:

1. **Record your Loom video**
2. **Get the video ID**:
   - Click "Share" on your Loom video
   - Click "Embed"
   - Copy the ID from the URL (e.g., `https://www.loom.com/embed/abc123xyz` → `abc123xyz`)
3. **Replace in the MDX file**:
   ```mdx
   src="https://www.loom.com/embed/YOUR_VIDEO_ID_HERE?hide_share=true&hideEmbedTopBar=true"
   ```

**Pages with Video Templates Ready**:
- ✅ Introduction (`introduction.mdx`) - "Quick Tour (2 Minutes)"
- ✅ Marketing (`prompts/marketing.mdx`) - "From Brief to Campaign Copy in 5 Minutes"
- ✅ Social Media (`prompts/social-media.mdx`) - "Create 10 Instagram Captions in 2 Minutes"
- ✅ ChatGPT Projects (`guides/chatgpt-projects.mdx`) - "Build Your First Project in 3 Minutes"

**Video Best Practices**:
- Keep videos under 5 minutes
- Show real Annoushka examples
- Use the Info callouts to guide what to include
- Add captions for accessibility

---

## How to Add More Visual Enhancements

### Adding Hero Images to Other Pages

**Pages that could use hero images**:
- `prompts/merchandising.mdx`
- `prompts/retail.mdx`
- `prompts/product-development.mdx`
- `prompts/hr.mdx`
- `getting-started/overview.mdx`

**Template**:
```mdx
---
title: Your Page Title
description: Your description
---

<img
  src="/images/JPG_2025/LOOK_XX_XXX copy.jpg"
  alt="Descriptive alt text"
  style={{ width: '100%', borderRadius: '12px', marginBottom: '2rem', maxHeight: '350px', objectFit: 'cover' }}
/>

## Your Content Starts Here
```

---

### Creating Image Galleries

**2-Column Layout**:
```mdx
<CardGroup cols={2}>
  <Card>
    <img src="/images/JPG_2025/image1.jpg" style={{ borderRadius: '8px' }} />
    <div style={{ padding: '1rem' }}>
      <h3>Caption Title</h3>
      <p>Description text here</p>
    </div>
  </Card>
  <Card>
    <img src="/images/JPG_2025/image2.jpg" style={{ borderRadius: '8px' }} />
    <div style={{ padding: '1rem' }}>
      <h3>Caption Title</h3>
      <p>Description text here</p>
    </div>
  </Card>
</CardGroup>
```

**3-Column Layout** (better for simple image grids):
```mdx
<CardGroup cols={3}>
  <Card>
    <img src="/images/JPG_2025/image1.jpg" />
  </Card>
  <Card>
    <img src="/images/JPG_2025/image2.jpg" />
  </Card>
  <Card>
    <img src="/images/JPG_2025/image3.jpg" />
  </Card>
</CardGroup>
```

---

### Using Visual Callouts

**With Images**:
```mdx
<Card>
  <img
    src="/images/JPG_2025/LOOK_XX_XXX copy.jpg"
    style={{ borderRadius: '8px', marginBottom: '1rem' }}
  />
  <h3>Key Takeaway Title</h3>
  <p>Important information or tip here that relates to the image above.</p>
</Card>
```

**Styled Callouts** (Already working in your pages):
```mdx
<Tip>
Your helpful tip here with an icon
</Tip>

<Warning>
Important warning or caution
</Warning>

<Info>
Useful information or context
</Info>

<Note>
Additional notes or considerations
</Note>
```

---

### Side-by-Side Content with Images

**Text + Image Layout**:
```mdx
<div style={{ display: 'grid', gridTemplateColumns: '1fr 1fr', gap: '2rem', alignItems: 'center' }}>
  <div>
    <h3>Your Content Title</h3>
    <p>Your text content here...</p>
  </div>
  <img
    src="/images/JPG_2025/LOOK_XX_XXX copy.jpg"
    style={{ borderRadius: '12px', width: '100%' }}
  />
</div>
```

---

### Tabs with Visual Content

**Great for before/after or different options**:
```mdx
<Tabs>
  <Tab title="Example 1">
    <img src="/images/JPG_2025/image1.jpg" style={{ borderRadius: '8px', marginBottom: '1rem' }} />
    Content for example 1
  </Tab>
  <Tab title="Example 2">
    <img src="/images/JPG_2025/image2.jpg" style={{ borderRadius: '8px', marginBottom: '1rem' }} />
    Content for example 2
  </Tab>
</Tabs>
```

---

## Brand Assets Reference

### Available Images

**Campaign Photos (19 total)**:
Located in `public/images/JPG_2025/`
- LOOK_01 through LOOK_15
- Some have black & white versions (`_blackwhite.jpg`)

**Logos (3 versions)**:
Located in `public/images/`
- `logo-dark.png` - For light backgrounds
- `logo-light.png` - For dark backgrounds
- `logo-gold.png` - Signature gold version

### Brand Guidelines

**PDF Location**: `public/brand guidelines/Annoushka Brand Guide.pdf`

This contains:
- Color palettes
- Typography rules
- Brand voice guidelines
- Visual style guidance

**Reference it in content**:
```mdx
<Info>
For full brand guidelines, see our [Brand Guide PDF](/brand%20guidelines/Annoushka%20Brand%20Guide.pdf)
</Info>
```

---

## Next Steps to Make it Even More Visual

### 1. Record Loom Videos (Priority!)
The templates are ready - you just need to record:
- Welcome tour (2 min)
- Marketing workflow demo (5 min)
- Social media captions demo (2 min)
- ChatGPT Projects setup (3 min)

### 2. Add More Hero Images
Add hero images to remaining prompt library pages:
- Merchandising
- Retail
- Product Development
- HR

### 3. Create "Example Output" Galleries
Show real examples of AI outputs with visuals:
- Social media caption examples with the images
- Email campaign examples styled like real emails
- Product description examples with product photos

### 4. Add Interactive Elements
- Accordions with images inside
- Collapsible sections with visual examples
- Step-by-step guides with screenshots

### 5. Create a Visual Resources Page
A dedicated page showcasing:
- All campaign images in a gallery
- Brand color swatches
- Typography examples
- Logo usage guidelines

---

## Testing Your Changes Locally

1. **Start the dev server**:
   ```bash
   cd annoushka-ai-hub
   mintlify dev
   ```

2. **Open in browser**: `http://localhost:3000`

3. **Check**:
   - Images load correctly
   - Fonts are applied
   - Layout looks good on mobile
   - Videos embed properly (when IDs added)

---

## Tips for Creatives

**What makes documentation visually appealing**:
1. ✅ **Real brand imagery** - Not stock photos (we've done this!)
2. ✅ **Consistent spacing** - Use margin/padding consistently
3. ✅ **Visual hierarchy** - Headers, callouts, cards for structure
4. ✅ **Brand fonts** - Masny + Contane (configured!)
5. ⏳ **Video tutorials** - Loom embeds ready to go
6. ⏳ **Real examples** - Show actual outputs with visuals
7. ⏳ **Color consistency** - Use brand colors throughout

**You've accomplished**: Items 1-4!
**Next priority**: Record those Loom videos!

---

## Quick Reference: Component Examples

**Hero Image**:
```mdx
<img src="/images/JPG_2025/LOOK_XX.jpg" style={{ width: '100%', borderRadius: '12px', marginBottom: '2rem', maxHeight: '350px', objectFit: 'cover' }} />
```

**Card with Image**:
```mdx
<Card>
  <img src="/images/JPG_2025/LOOK_XX.jpg" />
</Card>
```

**Video Embed**:
```mdx
<Frame caption="Your caption">
  <iframe src="https://www.loom.com/embed/VIDEO_ID" className="w-full aspect-video rounded-xl" frameBorder="0" allowFullScreen></iframe>
</Frame>
```

**Callout with Icon**:
```mdx
<Tip>Your tip here</Tip>
<Warning>Your warning</Warning>
<Info>Your info</Info>
```

**Card Grid**:
```mdx
<CardGroup cols={2}>
  <Card title="Title">Content</Card>
  <Card title="Title">Content</Card>
</CardGroup>
```

---

**Questions?** Test locally first, then record those videos to bring it all to life!
