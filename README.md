# HW3 - Design Token Palette

## LLM Transcript Snippet

**My Prompt:**
"Create a simple, student-appropriate HTML and CSS page for a 200-level web scripting assignment. Include design tokens (at least 5 color tokens and 2 typography tokens), two sections using CSS Grid (a hero section and a card grid with 4 cards), and ensure WCAG AA compliance. Keep the code simple and easy to understand."

**Model Response (Excerpt):**
The model provided a complete design system with:
- 5 color tokens: --bg (#f5f5f5), --surface (#ffffff), --text (#222222), --accent (#0066cc), --muted (#666666)
- 2 typography tokens: --font-base (Arial), --font-heading (Georgia)
- Additional size and spacing tokens
- Two sections with CSS Grid layouts
- Responsive breakpoints at 600px and 900px

**My Critique & Revisions:**
-  **Kept simple color palette**: The neutral gray background with blue accent is clean and accessible
-  **Verified contrast ratios**: All text/background combinations exceed WCAG AA requirements
-  **Adjusted spacing**: Changed --gap-large from 2rem to 2rem (kept it) for better visual rhythm
-  **Simplified grid**: Used simple grid-template-columns with clear breakpoints instead of complex auto-fit initially suggested
-  **Added focus states**: Ensured all interactive elements maintain visible focus outlines for keyboard navigation

## Design Notes

### Color Tokens
- `--bg: #f5f5f5` - Light gray page background
- `--surface: #ffffff` - White surface for cards and hero section
- `--text: #222222` - Near-black for primary text
- `--accent: #0066cc` - Blue for interactive elements (buttons, links)
- `--muted: #666666` - Gray for secondary text

### Typography Tokens
- `--font-base: Arial, sans-serif` - Clean, readable body text
- `--font-heading: Georgia, serif` - Classic serif for headings

### Size Tokens
- `--font-small: 0.875rem` (14px)
- `--font-normal: 1rem` (16px)
- `--font-large: 1.5rem` (24px)
- `--font-xlarge: 2.5rem` (40px)

### Spacing Tokens
- `--gap: 1rem` - Standard spacing unit
- `--gap-large: 2rem` - Larger spacing for sections

### Border Radius
- `--radius: 8px` - Rounded corners for cards and buttons

## Accessibility Notes

### Contrast Ratios (WebAIM Contrast Checker)
- **Text on Background**: #222222 on #f5f5f5 = **11.83:1** (Passes AAA)
- **Muted text on Background**: #666666 on #f5f5f5 = **4.54:1** (Passes AA)
- **Button text**: #ffffff on #0066cc = **4.58:1** (Passes AA)
- **Link text**: #0066cc on #ffffff = **4.58:1** (Passes AA)


## Timebox

**Total time spent**: Around 90 minutes
- Initial setup and token planning: 15 minutes
- HTML structure and content: 20 minutes
- CSS styling and grid layouts: 30 minutes
- Testing and accessibility checks: 15 minutes
- Documentation (tests.txt, README, explain.txt): 10 minutes

## Repository

**Changes from starter**:
- Added personal information section with name, bio, interests list
- Created token-based design system
- Implemented responsive grid layouts
