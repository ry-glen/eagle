# Ironclad Architectural Design System

## 1. Overview & Creative North Star
**Creative North Star: The Industrial Blueprint**
Ironclad Architectural is a design system built for permanence, reliability, and precision. It eschews the "soft" aesthetics of modern SaaS in favor of a high-contrast, editorial style that mirrors the durability of industrial materials. The system is defined by its mathematical rigor, utilizing a blueprint-inspired grid, sharp geometries, and a hierarchy that feels forged rather than painted. 

The aesthetic is characterized by:
*   **Architectural Weight:** Bold, heavy typography that anchors the page.
*   **Technical Transparency:** Use of "blueprint" background patterns to suggest engineering and planning.
*   **Intentional Asymmetry:** Breaking the standard grid with rotated images and overlapping elements to create a sense of dynamic motion within a rigid structure.

## 2. Colors
The palette is rooted in a "Patriotic Industrial" scheme—deep navy and vibrant crimson—offset by high-clarity neutrals.

*   **Primary (#002868):** Representing authority and stability. Used for main headlines and foundational UI elements.
*   **Secondary (#D21034):** The "Precision" color. Used for high-priority CTAs, accents, and critical status markers.
*   **The "No-Line" Rule:** Sectioning is achieved through color-blocking and surface shifts. Avoid 1px borders for defining content areas. Use `surface_container_low` (#f1f4f9) to separate sections from the pure white `surface` (#ffffff).
*   **Surface Hierarchy:**
    *   **Surface Lowest:** The pure canvas (#ffffff).
    *   **Surface Container Low:** Standard background for content sections.
    *   **Surface Container High:** Used for navigation bars and elevated cards.
*   **Signature Textures:** Utilize the "Blueprint Grid"—a subtle 24px linear gradient overlay—at 3-5% opacity to add industrial texture to hero and CTA sections.

## 3. Typography
The typography scale leverages high-contrast weights and technical geometric forms.

**Headline Font: Space Grotesk**
A idiosyncratic sans-serif with geometric roots. Used for all Display and Headline levels to convey a "tech-industrial" feel.
*   **Display Large (8rem / 128px):** Reserved for ultra-short, high-impact hero text. Tracking should be tightened (-0.05em).
*   **Display Medium (3.75rem / 60px):** For main section titles.
*   **Headline Small (1.5rem / 24px):** Used for card titles and sub-headings.

**Body & Label Font: Public Sans**
A strong, neutral typeface designed for clarity.
*   **Body Large (1.125rem / 18px):** Standard reading size with generous line height (1.6) for legibility.
*   **Label/Small (0.75rem / 12px):** Used for "Client Satisfaction Reports" or data tags, always set in All-Caps with 10% tracking.

## 4. Elevation & Depth
Depth in Ironclad Architectural is conveyed through **Tonal Layering** and **Aggressive Shadows** rather than traditional bevels.

*   **The Layering Principle:** Stack components using escalating surface tiers. A card on a `surface_container_low` background should use `surface_container_lowest` (#ffffff).
*   **Ambient Shadows:**
    *   **Low (shadow-sm):** For persistent interface elements.
    *   **Medium (shadow-lg):** For primary buttons and interactive cards.
    *   **Extreme (shadow-2xl):** Specifically for "Hero" images or key testimonials to create significant visual lift and overlapping depth.
*   **Glassmorphism:** Use `bg-white/95` with `backdrop-blur-sm` for fixed navigation bars to maintain content awareness during scrolling.

## 5. Components
### Buttons
*   **Primary:** High-saturation `secondary` color, `rounded-lg` (0.25rem), bold typography. Must include a `shadow-lg` colored with a 20% opacity of the button's background.
*   **Tertiary:** Outline-style with `border-primary/10`, uppercase tracking for a technical look.

### Cards & Bento Grid
*   **Testimonial Cards:** Large, flat-color blocks (`primary` or `secondary`) or white blocks with `shadow-sm`. 
*   **Decorative Quotes:** Use massive, low-opacity (50%) quote marks in the corner as a structural graphic element.

### Inputs & Selects
*   **Search/Input Fields:** Use `shadow-inner` on `surface_container_low` backgrounds to create a "recessed" industrial look.

## 6. Do's and Don'ts
*   **Do:** Use 2-degree rotations on featured images to break the rigid grid.
*   **Do:** Use high-contrast color blocks (e.g., White text on Primary Blue) for entire sections.
*   **Don't:** Use rounded corners exceeding 8px (0.5rem). The system must remain sharp and "Ironclad."
*   **Don't:** Use generic icons. Use "Material Symbols Outlined" with specific `wght: 400` and `FILL: 1` for a consistent architectural weight.
*   **Do:** Leverage the "Blueprint Grid" opacity for background depth.