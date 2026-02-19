# Masters Barbershop (GA) — Demo Website Redesign Plan (Execution-Ready)

## 1) Project Intent
This demo redesign should look and feel like a real production launch candidate, not just a style concept. The primary business outcome is to increase completed bookings from local traffic, especially mobile users searching for nearby barbers.

### Primary goals
1. Increase appointment bookings through a fast, low-friction flow.
2. Improve trust and credibility through authentic visuals, reviews, and barber profiles.
3. Clarify services/pricing to reduce pre-booking uncertainty.
4. Improve local discoverability (SEO + map visibility + consistent NAP).

### Success metrics for the demo
- +20% improvement in **Book Now CTA click-through rate** (compared to current site baseline).
- +15% increase in **booking start rate** from mobile traffic.
- <2.5s Largest Contentful Paint on 4G mobile for key pages.
- Lighthouse targets: 90+ Performance, 95+ Accessibility, 90+ SEO.

---

## 2) Audience + User Jobs

### Core audience segments
- **Young professionals (18–35):** want sharp cuts/fades and quick online booking.
- **Returning locals:** want consistency and their preferred barber.
- **Parents:** need clear kids’ pricing and convenient scheduling.
- **Walk-in users:** need instant clarity on wait time/hours/contact.

### Top user jobs to solve
- “Can I get the cut I want, at a clear price, with someone skilled?”
- “Can I book quickly from my phone without creating friction?”
- “Is this place reputable and nearby?”

---

## 3) Brand + Visual System (Demo)

### Visual tone
- Premium but approachable
- Masculine and modern
- Local and authentic

### Color tokens
- `--color-bg-dark: #111111`
- `--color-accent-gold: #C89B3C`
- `--color-bg-light: #F7F7F5`
- `--color-text-dark: #222222`
- `--color-text-light: #FFFFFF`
- `--color-cta: #0E7A4B`
- `--color-danger: #B3261E` (form/error states)

### Typography system
- Heading font: **Bebas Neue** or **Oswald**
- Body/UI font: **Inter**
- Type scale recommendation:
  - H1: 48/56 (desktop), 34/40 (mobile)
  - H2: 36/44, 28/34
  - H3: 28/34, 22/28
  - Body: 18/28, 16/24
  - Small/UI: 14/20

### Component styling notes
- Buttons: 10–12px radius, semibold text, clear hover/focus state.
- Cards: subtle shadow + thin border for depth on light sections.
- Section spacing: 96px desktop / 64px tablet / 40px mobile.

---

## 4) Sitemap + Navigation Strategy

## Primary sitemap
1. Home
2. Services & Pricing
3. Barbers
4. Gallery
5. Reviews
6. Contact
7. Book Now

## Header behavior
- Sticky header with persistent **Book Now** CTA.
- Mobile: compact top bar + slide-out menu + floating bottom CTA.
- Include tap targets >= 44px for accessibility.

## Footer content
- NAP (name, address, phone)
- Hours summary
- Quick links
- Social links
- “Book Now” repeated CTA

---

## 5) Page Blueprints (High-Fidelity Content Plan)

## Home
### A. Hero (above the fold)
- Visual: in-shop action photo/video loop.
- Headline: **“Sharp Cuts. Real Craft. Right Here in Georgia.”**
- Subtext: “Book with trusted local barbers for fades, beard grooming, and clean finishes.”
- CTAs:
  - Primary: **Book Appointment**
  - Secondary: **View Services**

### B. Trust strip
- “Top-rated local barbershop”
- “Walk-ins welcome”
- “Open late on select days” (only if accurate)
- Optional: “4.8★ from local clients”

### C. Featured services (4 cards)
- Haircut
- Skin Fade
- Beard Trim
- Kids Cut
Each card: short description + starting price + duration.

### D. Meet the team preview
- 2–3 barbers with photo, specialty, and quick booking links.

### E. Social proof
- Review carousel with rating average and source badges.

### F. Local convenience block
- Map snippet + “Call now” + today’s hours + “Get Directions.”

---

## Services & Pricing
- Group by category: Haircuts, Beard, Combo, Add-ons.
- Service cards include:
  - Name
  - Description
  - Duration
  - Starting price
  - “Book this service” action
- FAQ accordion:
  - Walk-ins vs appointments
  - Late arrival policy
  - Accepted payments
  - Cancellation policy
- Sticky mobile booking CTA always visible.

---

## Barbers
- Profile cards per barber:
  - Headshot
  - Name
  - Specialty (e.g., skin fades, beard sculpting)
  - Years of experience
  - Social proof snippet (optional)
  - CTA: “Book with [Name]”
- Optional filters: Fades / Beard / Kids / Fast appointments.

---

## Gallery
- Masonry or balanced grid of haircut outcomes.
- Optional tags: Fade, Taper, Beard, Kids.
- Lightbox with keyboard support and alt text.
- Optional Instagram strip for freshness.

---

## Reviews
- Rating summary module (average + count).
- 6–12 curated testimonials.
- “See all reviews” external link.
- CTA pair:
  - “Book your visit”
  - “Leave a review”

---

## Contact
- Address, phone, hours, and map embed.
- Parking note + landmark helper text.
- Contact form fields: Name, Phone/Email, Message.
- If possible, add “Current wait estimate” banner for walk-ins.

---

## Book Now
- Preferred: embedded booking widget (Square/Booksy/Fresha/etc.).
- Demo fallback: pseudo flow
  1. Select service
  2. Select barber
  3. Select time
  4. Enter contact info
  5. Confirmation screen
- Include cancellation and no-show policy text beneath CTA.

---

## 6) Conversion & UX Requirements

### Critical conversion elements
- Persistent top-right “Book Now.”
- Floating mobile “Book Now” button.
- Pricing visible early (homepage + services).
- Fast path: Home → Service → Barber → Time.

### Friction reducers
- Don’t require account creation before timeslot selection.
- Auto-fill capable forms.
- Visible trust cues near conversion points.

### Recommended microcopy
- “Reserve your chair in under 60 seconds.”
- “Walk-ins welcome, appointments prioritized.”
- “Need help choosing? Call us now.”

---

## 7) Local SEO Plan
- Page titles with city intent (e.g., “Masters Barbershop | Barbershop in [City], GA”).
- Service pages include local modifiers naturally in copy.
- LocalBusiness schema with:
  - Name
  - Address
  - Phone
  - Opening hours
  - Aggregate rating (if compliant)
- Ensure NAP consistency with Google Business Profile and social channels.
- Add internal links between Services, Barbers, and Book Now.

---

## 8) Accessibility + Performance Standards

### Accessibility checklist
- Color contrast meets WCAG AA.
- Visible focus rings on all interactive elements.
- Proper heading hierarchy (single H1/page).
- Descriptive alt text for gallery/barber images.
- Form labels and error messaging with ARIA support.

### Performance checklist
- Images served as AVIF/WebP with responsive sizes.
- Lazy-load below-the-fold media.
- Use `font-display: swap`.
- Minify CSS/JS and defer non-critical scripts.
- Preconnect to booking/widget domains if embedded.

---

## 9) Content Collection Checklist (Before Build)
- Official logo files (SVG + PNG)
- 15–25 high-quality haircut images
- 3–8 shop/team photos
- Verified service list, duration, and prices
- Barber bios + specialties + headshots
- Hours, holiday exceptions, and contact info
- 10+ approved review snippets

---

## 10) Build & Delivery Plan (2-Week Demo Sprint)

### Week 1
1. Discovery + content validation
2. Wireframes (Home, Services, Book Now)
3. Visual direction approval
4. High-fidelity homepage + shared components

### Week 2
5. Complete page designs (desktop + mobile)
6. Implement responsive front-end demo
7. QA (SEO, a11y, performance, form flow)
8. Stakeholder walkthrough + revision pass

---

## 11) Optional Premium Demo Features
- “Book your usual barber” quick action for return visitors.
- Style inspiration recommender (“Show me fades under 30 min”).
- Loyalty/promo banner module.
- SMS reminder mock flow.
- Gift cards section.

---

## 12) Definition of Done
The redesign demo is complete when:
1. All core pages are responsive and connected.
2. Booking CTAs are consistently present and functional.
3. Services/pricing are clear and scannable.
4. Barbers, gallery, and reviews establish trust.
5. SEO metadata + schema placeholders are implemented.
6. Accessibility and performance targets are met or documented.
7. Demo is handoff-ready for production development.
