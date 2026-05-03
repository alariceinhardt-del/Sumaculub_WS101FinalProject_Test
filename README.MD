# Piapi III FLA — Farmers & Laborers Association Website

---

## Table of Contents

* [Creator](#creator)
* [Project Overview](#project-overview)
* [AI Usage Documentation](#ai-usage-documentation)

---

# Creator

This project was created by **Cyrille Cezar A. Sumaculub** of **BSIT-3B** as partial requirement for the course WS-101.

---

# Project Overview

The **Farmers & Laborers Association of Barangay Piapi III Official Website** is a multi-page informational website created for a real barangay-level farmers association located in Hamtic, Antique.

The website serves as the association’s digital presence and includes:

* Homepage
* About Page
* Programs Page
* Events Page
* Gallery
* Membership Application Form

---

# Framework Used

* HTML5
* CSS3
* Vanilla JavaScript
* PHP
* Laragon

No external frontend frameworks were used.

---

# AI Usage Documentation

This section documents how AI tools were used throughout the development process of the project.

---

## 1. Context Loading / Silent Review

### Purpose

To allow the AI to understand the existing codebase before asking specific implementation questions.

### Prompt Used

```txt
shut up for review until i say so, only reply with ok
```

### Application

The homepage HTML was pasted into the AI conversation without requesting any output. This allowed the AI to absorb the existing structure, naming conventions, CSS variables, and component patterns before later discussions.

No code was generated during this stage.

---

## 2. Homepage Structure Generation

### Purpose

To generate an initial homepage structure for the association website.

### Prompt Used

```txt
make me a website for a farmers association in hamtic antique
```

### Application

The AI generated a homepage containing:

* Hero Section
* About Preview
* Mission & Values
* Program Cards
* Events Section
* Gallery
* Testimonials
* CTA Section
* Footer

Most textual content was later rewritten manually to match the real organization.

---

## 3. Color Palette Guidance

### Purpose

To find an earthy color palette appropriate for an agricultural association website.

### Prompt Used

```txt
use earthy tones, like dark green, brown, amber, cream. nothing blue nothing purple
```

### Application

The AI generated a set of CSS variables for the color palette. Several values were later adjusted manually to improve readability and visual balance.

---

## 4. Typography Pairing

### Purpose

To choose fonts that matched the intended visual identity.

### Prompt Used

```txt
the font should feel old but clean. like a newspaper but modern
```

### Application

The AI suggested:

* Cormorant Garamond
* DM Sans
* DM Mono

Typography sizing, spacing, and scaling were later manually refined.

---

## 5. Paper Texture Background Effect

### Purpose

To create a subtle paper-like texture using only CSS.

### Prompt Used

```txt
add a paper texture to the background
```

### Application

The AI generated an inline SVG noise texture using `feTurbulence` within a pseudo-element.

Opacity and layering behavior were later manually adjusted.

---

## 6. Navbar Scroll Behavior

### Purpose

To create a transparent navbar that changes appearance while scrolling.

### Prompt Used

```txt
make the navbar transparent at top then turn dark when scrolled
```

### Application

The AI generated the scroll listener and `.scrolled` state styling.

Additional refinements were later added manually.

---

## 7. Hero Carousel

### Purpose

To implement a lightweight custom hero image carousel.

### Prompt Used

```txt
add a carousel to the hero with farm images
```

### Application

The AI generated the carousel logic using:

* `translateX`
* Dot navigation
* Auto-advance using `setInterval`

Image assets and timing adjustments were customized manually.

---

## 8. Scroll Reveal Animations

### Purpose

To animate elements when entering the viewport.

### Prompt Used

```txt
scroll reveal — make elements fade up when they enter the viewport
```

### Application

The AI generated the Intersection Observer setup.

Custom animation variants and stagger timing were later implemented manually.

---

## 9. About Page Timeline

### Purpose

To create a vertical timeline for the association history.

### Prompt Used

```txt
make the about page with a timeline of the association history
```

### Application

The AI generated the structural timeline layout.

All historical content and milestone descriptions were written manually.

---

## 10. Officer Cards

### Purpose

To design officer profile cards matching the website’s visual identity.

### Prompt Used

```txt
about page — add officer cards with their photos and roles
```

### Application

The AI generated the layout structure while all real names, descriptions, and images were added manually.

---

## 11. Membership Multi-Step Form

### Purpose

To structure the online membership application form.

### Prompt Used

```txt
member form — make it a multi-step form with a progress bar
```

### Application

The AI generated:

* Step logic
* Progress bar system
* Navigation behavior

Form fields, validation rules, and review logic were implemented manually.

---

## 12. PHP Conversion for Laragon

### Purpose

To convert the static frontend into a PHP-compatible project for local hosting.

### Prompt Used

```txt
this is only front end / how do i convert this to php? whats the extension / so its laragon compatible and can be transmitted even in local host on the same wifi
```

### Application

The AI explained:

* File conversion process
* Folder structure
* Link adjustments
* Basic PHP handling

All project-wide path corrections and LAN testing were performed manually.

---

## 13. PHP Form Processing

### Purpose

To process membership submissions server-side.

### Prompt Used

```txt
the form should save submissions to a file and show a reference code
```

### Application

The AI generated:

* `$_POST` handling
* Input sanitization
* Reference generation
* File saving logic

The final formatting and success state UI were manually customized.

---

## 14. Responsive Layout Debugging

### Purpose

To fix responsive layout issues across multiple pages.

### Prompt Used

```txt
the gallery grid breaks on mobile, the first image is still taking 2 columns
```

### Application

The AI identified that the grid span rules were still active inside the mobile breakpoint.

Reset rules were added manually to correct the layout.

---

## 15. Mobile Navigation Overlay

### Purpose

To build a full-screen mobile navigation menu.

### Prompt Used

```txt
make a mobile menu that covers the whole screen
```

### Application

The AI generated:

* Overlay structure
* Animation system
* Close button behavior
* Animated link transitions

Additional styling and timing adjustments were later customized manually.

---

## 16. Form Validation System

### Purpose

To implement non-intrusive custom validation states.

### Prompt Used

```txt
form — custom error states with red borders and messages
```

### Application

The AI generated reusable validation helper functions and error styles.

Field requirements and additional UX improvements were later implemented manually.

---

## 17. CSS Learning & Explanations

### Purpose

To better understand modern CSS techniques used within the project.

### Topics Asked

* `:has()` selector
* Custom radio buttons
* Sticky positioning
* Media query behavior
* Grid span resets

### Application

These discussions helped improve understanding of newer CSS features and layout behavior.

---

## 18. Sticky Event Filter Bar

### Purpose

To keep the events category filter visible while scrolling.

### Prompt Used

```txt
events page — add a filter bar that sticks below the navbar
```

### Application

The AI explained the use of `position: sticky` with a top offset matching the navbar height. The filter styling, categories, and JavaScript filtering logic were implemented manually.

---

## 19. Featured Event Card

### Purpose

To create a larger highlighted event layout different from standard event cards.

### Prompt Used

```txt
events page — featured event should be a big two-column card
```

### Application

The AI generated the grid structure and visual layout. Event content, metadata, and imagery were added manually.

---

## 20. Past Events List Layout

### Purpose

To organize previous events into a readable structured list.

### Prompt Used

```txt
events page — past events as a list with date columns
```

### Application

The AI created the layout skeleton using CSS grid while all event information and descriptions were manually written.

---

## 21. Programs Page Step Section

### Purpose

To visually explain the membership or program workflow.

### Prompt Used

```txt
programs page — add a how-it-works section with numbered steps and a connecting line
```

### Application

The AI created the connecting line system and numbered step structure. Titles, descriptions, and responsive adjustments were manually implemented.

---

## 22. Programs Statistics Banner

### Purpose

To display organization statistics in a visually strong banner section.

### Prompt Used

```txt
programs page — stats band with big numbers
```

### Application

The AI adapted an existing banner layout pattern into a statistics display. All numerical data and labels were manually chosen.

---

## 23. Membership Perks Strip

### Purpose

To display membership benefits in a horizontal information strip.

### Prompt Used

```txt
member page — add an amber perks strip between the header and form
```

### Application

The AI created the flexbox structure while all perk items and responsive fixes were manually customized.

---

## 24. Sticky Membership Sidebar

### Purpose

To keep important membership information visible during form completion.

### Prompt Used

```txt
member page — sticky left panel with benefits list
```

### Application

The AI suggested sticky positioning and offset behavior. Final spacing adjustments and mobile fallback behavior were manually refined.

---

## 25. Review Step Logic

### Purpose

To display submitted form information before final submission.

### Prompt Used

```txt
form step 3 — review grid that auto-fills from previous steps
```

### Application

The AI described the general implementation strategy while the actual JavaScript logic and field rendering were written manually.

---

## 26. Decorative Top Accent Line

### Purpose

To add subtle visual separation at the top of the page.

### Prompt Used

```txt
put a thin amber line at the very top of the page
```

### Application

The AI generated a pseudo-element gradient line. Layering fixes were later manually added.

---

## 27. Value Card Hover Effects

### Purpose

To improve interaction feedback in the values section.

### Prompt Used

```txt
values section — make the cards flip to dark background on hover
```

### Application

The AI suggested avoiding unnecessary 3D transforms and recommended simpler background transitions. Hover animations were manually refined.

---

## 28. Mobile Navigation Animation Timing

### Purpose

To improve the pacing of animated mobile navigation links.

### Prompt Used

```txt
mobile menu links should slide in from the left one by one
```

### Application

The AI generated staggered animations using incremental delays. Timing values were later manually adjusted.

---

## 29. Navbar Styling Debugging

### Purpose

To identify inconsistent navigation styling across pages.

### Prompt Used

```txt
why is the about page nav always dark even when im at the top
```

### Application

The AI identified an incorrectly applied background property. Removing the property restored consistent behavior.

---

## 30. Scroll-To-Top Button Debugging

### Purpose

To determine why the scroll button was not appearing on one page.

### Prompt Used

```txt
scroll to top button not showing on about page
```

### Application

The AI guided the debugging process by checking whether the button element existed in the page structure.

---

## 31. Responsive Breakpoint Consistency

### Purpose

To ensure responsive behavior remained consistent across all pages.

### Prompt Used

```txt
are my media query breakpoints the same across all pages
```

### Application

The AI suggested standardizing breakpoint values. Each page was then manually audited and corrected.

---

## 32. Gallery Mobile Layout Fix

### Purpose

To repair gallery layout issues on smaller screens.

### Prompt Used

```txt
the gallery grid breaks on mobile, the first image is still taking 2 columns
```

### Application

The AI explained how span rules continued applying under media queries. Reset rules were manually added.

---

## 33. CSS :has() Selector Explanation

### Purpose

To understand modern CSS parent selector behavior.

### Prompt Used

```txt
what does :has(input:checked) do, is it safe to use
```

### Application

The AI explained how the selector reacts to child element states and discussed browser compatibility.

---

## 34. Custom Radio Button System

### Purpose

To understand how CSS-only custom radio buttons function.

### Prompt Used

```txt
how do the custom radio buttons work without javascript
```

### Application

The AI explained the interaction between hidden inputs, labels, and checked states.

---

## 35. Background Texture Optimization

### Purpose

To reduce visual noise caused by the paper texture effect.

### Application

Opacity values and layering behavior were manually adjusted after testing on mobile devices.

---

## 36. Hero Animation Timing Refinement

### Purpose

To improve the pacing of hero entrance animations.

### Application

Animation delays generated by AI were manually tightened to create a faster and cleaner sequence.

---

## 37. LAN Accessibility Testing

### Purpose

To verify the project worked across devices on the same WiFi network.

### Application

LAN access was manually tested through Laragon and firewall troubleshooting was performed without AI assistance.

---

## 38. File Structure Organization

### Purpose

To maintain manageable styling and page organization.

### Application

AI-generated comments and manually added notes helped navigate large CSS files during later revisions.

---

## 39. Base Tag Navigation Bug

### Purpose

To determine why internal links opened in new tabs.

### Prompt Used

```txt
the homepage links are opening in new tabs, is the base tag causing this
```

### Application

The AI confirmed that the base tag configuration was forcing links into new tabs. The tag was removed manually.

---

## 40. PHP Submission Reference Formatting

### Purpose

To improve the readability of generated submission reference codes.

### Application

The AI generated the original reference logic while the final format was manually redesigned for readability.

---

## 41. Overall AI Contribution Summary

### Purpose

To summarize the role AI played throughout development.

### Application

AI primarily assisted with:

* Structural scaffolding
* Debugging guidance
* CSS explanations
* JavaScript boilerplate
* PHP handling
* UI layout suggestions
* Animation setup
* Responsive troubleshooting

Final implementation decisions, refinements, testing, responsiveness, content writing, and project-specific customization were completed manually.

---