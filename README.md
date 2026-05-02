# TailwindCSS Design Conversion

## Overview

This project converts provided design assets into a functional responsive web layout using TailwindCSS.

The source design materials are expected to include:

- PNG files for each page or screen.
- A PDF that documents exact sizing requirements.

The implementation should closely match the provided PNG designs across layout, spacing, typography, and responsive behavior.

## Requirements

- Convert all supplied design pages into working web layouts.
- Use TailwindCSS utility classes as the primary styling method.
- Convert all pixel-based dimensions from the PDF into REM units compatible with TailwindCSS.
- Add custom CSS only when a design requirement cannot reasonably be achieved with TailwindCSS utilities.
- Support responsive layouts for mobile, tablet, and desktop viewport sizes.

## Pixel to REM Conversion

Use `16px = 1rem` as the base conversion rule.

Examples:

| Pixels | REM |
| --- | --- |
| 4px | 0.25rem |
| 8px | 0.5rem |
| 12px | 0.75rem |
| 16px | 1rem |
| 24px | 1.5rem |
| 32px | 2rem |
| 48px | 3rem |
| 64px | 4rem |

When possible, use TailwindCSS spacing, sizing, typography, and breakpoint utilities that already map to the required REM values. If the exact value is not available in the default Tailwind scale, use Tailwind arbitrary values with REM units, for example:

```html
<div class="mt-[1.125rem] w-[17.5rem]">
```

## Styling Guidelines

- Prefer TailwindCSS utilities for spacing, sizing, colors, layout, typography, borders, shadows, and responsive states.
- Use semantic HTML where practical.
- Keep custom CSS minimal and limited to cases TailwindCSS cannot express cleanly.
- Preserve the visual hierarchy shown in the PNG files.
- Match font sizes, line heights, weights, colors, margins, padding, and element dimensions from the design references.
- Implement responsive behavior intentionally instead of only scaling the desktop design down.

## Responsive Targets

The layout must work correctly on:

- Mobile screens.
- Tablet screens.
- Desktop screens.

Use TailwindCSS responsive prefixes such as `sm:`, `md:`, `lg:`, and `xl:` as appropriate for the design.

## Acceptance Criteria

- [ ] All provided design pages are converted into functional web layouts using TailwindCSS.
- [ ] Pixel dimensions from the PDF are translated into TailwindCSS-compatible REM units.
- [ ] The implementation matches the visual layout, spacing, and typography shown in the PNG files.
- [ ] Custom CSS is used only where TailwindCSS utility classes cannot meet the design requirement.
- [ ] Layouts are responsive and function correctly on mobile, tablet, and desktop views.

## Delivery Notes

The completed files should be ready within the requested two-day timeline and should include all source code needed to run, review, and verify the TailwindCSS implementation.
