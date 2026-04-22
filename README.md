# MA Tech Email Templates Guide

## Overview
Professional, brand-aligned email templates for MA Tech. All templates are responsive, mobile-optimized, and follow industry best practices for software companies.

---

## 📋 Templates Included

### 1. **Welcome Email** (`welcome-email.html`)
**When to use:** First contact with new clients/customers
- Warm greeting and introduction
- Value proposition summary
- Call-to-action for next steps
- Professional tone to build trust

### 2. **Project Update Email** (`project-update-email.html`)
**When to use:** Regular progress reports during active projects
- Progress statistics (% complete, timeline)
- Milestone breakdown with status indicators
- Achievement summary
- Clear next steps
- Engagement CTA

### 3. **Proposal / Quote Email** (`proposal-quote-email.html`)
**When to use:** Sending quotes, proposals, or pricing
- Professional header with proposal reference number
- Clear deliverables breakdown
- Itemized pricing
- Project timeline with milestones
- Strong call-to-action for acceptance
- Discussion option

### 4. **Invoice Email** (`invoice-email.html`)
**When to use:** Payment requests
- Clear invoice number and dates
- Itemized breakdown with amounts
- Payment due date prominently displayed
- Multiple payment method options
- Payment button/link
- Professional, business tone

### 5. **Support/Help Email** (`support-help-email.html`)
**When to use:** Responding to support tickets
- Empathetic greeting
- Clear problem identification
- Step-by-step solution guide
- Code examples if applicable
- FAQ section
- Escalation option for complex issues
- Knowledge base links

### 6. **Project Completion Email** (`project-completion-email.html`)
**When to use:** Project delivery and launch
- Celebratory tone
- Complete list of deliverables
- Next steps guidance
- Documentation and resources
- Upsell opportunity for Phase 2
- Testimonial request

---

## 🎨 Brand Colors Used

- **Primary Dark:** `#0F172A` (Navy Blue)
- **Accent (Main):** `#0D9488` (Teal) - Used for buttons, highlights, borders
- **Accent Hover:** `#0F766E` (Dark Teal)
- **Secondary:** `#6366F1` (Indigo)
- **Background:** `#F8FAFC` (Light Blue-Gray)
- **Text Primary:** `#0F172A` (Navy)
- **Text Secondary:** `#475569` (Slate Gray)
- **Success:** `#10B981` (Green)
- **Warning:** `#F59E0B` (Orange)
- **Error:** `#EF4444` (Red)

---

## 🔧 How to Use These Templates

### Step 1: Add Your Logo
Replace `LOGO_URL_HERE` with your actual logo URL:
```html
<img src="https://your-domain.com/logo.png" alt="MA Tech" class="logo">
```

**Logo Optimization Tips:**
- Keep logo **150-200px width** for best visibility
- Use **PNG format** (better compression than JPG)
- Target file size: **20-50KB**
- For retina displays, use 2x resolution at half display size
- Recommended: Use SVG format (smallest file size, scalable)

**Option: Base64 Embed (No External Requests)**
If you want to embed the logo directly in the email:
1. Optimize your PNG logo to < 30KB
2. Convert to Base64: Use online tool or command:
   ```bash
   base64 logo.png
   ```
3. Replace in template:
   ```html
   <img src="data:image/png;base64,[BASE64_STRING_HERE]" alt="MA Tech" class="logo">
   ```

### Step 2: Customize Content
- Replace `[Client Name]` with actual client data
- Update project details, amounts, timelines
- Add your real contact information
- Include actual links to your website, documentation, etc.

### Step 3: Update Footer Links
Replace placeholder links:
- Website: `https://matech.com` → Your actual domain
- Email: `hello@matech.com` → Your support email
- Social media links with your profiles
- Contact information

### Step 4: Test Before Sending
- Test in major email clients (Gmail, Outlook, Apple Mail)
- Use Email on Acid or Litmus for cross-client testing
- Check mobile responsiveness
- Test all buttons and links
- Verify images load correctly

---

## 💡 Best Practices

### Mobile Optimization ✅
- All templates are mobile-responsive (600px max width)
- Text scales appropriately on smaller screens
- Buttons are touch-friendly (minimum 44px height)
- Images are responsive with `height: auto`

### Email Client Compatibility ✅
- Uses `table` layouts (more compatible than CSS Grid)
- Inline CSS for better client support
- Avoids complex CSS animations
- All colors are hex codes (no RGB)

### Accessibility ✅
- `alt` attributes on all images
- Semantic heading hierarchy
- Sufficient color contrast ratios
- Link descriptions are clear

### Performance ✅
- Minimal external dependencies
- No JavaScript (not supported in emails)
- Base64 embedded images reduce HTTP requests
- Optimized file sizes

---

## 🎯 Design Elements Explained

### Buttons
**Primary CTA (Teal):**
```html
<a href="#" class="cta-button">Action Text</a>
```
- Color: `#0D9488` (brand teal)
- Padding: 12-14px vertical, 32-40px horizontal
- Rounded corners: 8px
- Font weight: 600 (semi-bold)

### Section Boxes
- Light background: `#F8FAFC`
- Left border: 4px `#0D9488` (accent)
- Radius: 8px
- Padding: 20px

### Status Badges
- Success (Green): `#D1FAE5` background, `#065F46` text
- In Progress (Blue): `#DBEAFE` background, `#1E40AF` text
- Upcoming (Gray): `#F3F4F6` background, `#374151` text

---

## 📧 Email Integration Tips

### Sending Platforms
These templates work with:
- ✅ SendGrid
- ✅ Mailchimp
- ✅ Sendgrid
- ✅ Amazon SES
- ✅ Direct SMTP (Gmail, Office 365)
- ✅ Any custom email service

### HTML Template Variables
Use your email service's template syntax:
```html
<!-- For SendGrid -->
{{ client_name }}
{{ project_name }}
{{ total_amount }}

<!-- For Mailchimp -->
*|FNAME|*
*|COMPANY|*
*|TOTAL|*
```

### Personalization Best Practices
- Always use recipient name: "Hi [Name]," not "Hi there,"
- Include specific project details
- Reference previous conversations
- Use their domain/company name when possible

---

## ⚡ Quick Customization Checklist

Before sending any template:
- [ ] Replace `LOGO_URL_HERE` with actual logo
- [ ] Update all `#` placeholder links
- [ ] Replace `[Client Name]` with real name
- [ ] Update email addresses (support, hello@)
- [ ] Add actual phone number if applicable
- [ ] Update year in footer copyright
- [ ] Verify all content for accuracy
- [ ] Test all links work
- [ ] Check email preview on mobile
- [ ] Send test email to yourself first

---

## 🎨 Font Family
All templates use **Inter** with fallbacks:
```css
font-family: 'Inter', 'Segoe UI', 'Roboto', sans-serif;
```

Inter is modern, clean, and highly readable in emails. Make sure to import it if not available on email client (or include `<link>` tag).

---

## 💌 Email Subject Line Suggestions

| Template | Subject Examples |
|----------|-----------------|
| Welcome | "Welcome to MA Tech! 🚀" or "Let's Build Something Great Together" |
| Project Update | "[PROJECT NAME] - Progress Update #2" or "Great Progress on Your Project!" |
| Proposal | "Proposal for [PROJECT] - Ready to Discuss" |
| Invoice | "Invoice #INV-2026-0042 Due on April 10" |
| Support Response | "We've Got a Solution for You!" |
| Completion | "🎉 Your Project is Live!" |

---

## 📊 Typography Scale

- **Headers:** 20-28px, Weight 600-700
- **Body Text:** 14px, Weight 400, Color #475569
- **Section Titles:** 12-14px (uppercase), Weight 600, Tracking 0.5px
- **Footer:** 12px, Weight 400, Color #94A3B8

---

## 🔐 Security Notes

- All links should use HTTPS
- Remove any sensitive client data before archiving templates
- Don't include passwords or API keys in emails
- Use proper tracking pixels if you need to track opens
- Comply with CAN-SPAM and GDPR regulations

---

## 📱 Responsive Breakpoints

- Desktop: Default (600px max-width)
- Tablet: Media query at 600px
- Mobile: Font sizes reduce by ~10-15%
- Buttons stack on mobile if needed

---

## 🚀 Next Steps

1. **Create Logo Variants:**
   - White version (for dark headers)
   - Teal version (standard)
   - Inline SVG version (smallest file size)

2. **Set Up Email Service:**
   - Configure sender authentication (SPF, DKIM, DMARC)
   - Set up unsubscribe lists
   - Configure reply-to address

3. **Create Template Variables:**
   - Set up dynamic content blocks
   - Create reusable snippets
   - Build template library in your email service

4. **A/B Testing:**
   - Test subject lines
   - Test button colors
   - Test CTA copy
   - Track metrics (open rate, click rate, conversion rate)

---

## 📞 Support

For questions about these templates or custom modifications, contact the MA Tech development team.

Last Updated: April 3, 2026
