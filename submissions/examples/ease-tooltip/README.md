# Pure CSS Tooltips (`.ease-tooltip`)

## Description
This submission fulfills Issue #57085. Tooltips are essential for UI clarity, but requiring a JavaScript library just to show a small text box on hover is overkill.

This component provides a robust, fully-featured tooltip system using only CSS pseudo-elements (`::before` and `::after`) and HTML `data-*` attributes.

## Features
- **Zero JavaScript:** Completely CSS driven.
- **Data-Attribute Driven:** The text of the tooltip is set directly in the HTML via the `data-tooltip="My Text"` attribute.
- **Four Positions:** Includes modifier classes for all standard directions: `.ease-tooltip-top`, `.ease-tooltip-bottom`, `.ease-tooltip-left`, and `.ease-tooltip-right`.
- **Animated:** Features a smooth fade-in and scale-up animation on `:hover` or `:focus-visible`.
- **Accessible:** Respects `prefers-reduced-motion` by removing the scale-up transition for users with vestibular disorders.

## Usage
Simply add the `.ease-tooltip` and directional class to any element, and specify the text in the `data-tooltip` attribute:
```html
<button class="ease-tooltip ease-tooltip-top" data-tooltip="This is a pure CSS tooltip!">Hover Me</button>
```

## Files Included
- `demo.html`: An interactive demo showing all four tooltip directions.
- `style.css`: The component CSS, ready to be integrated into the core framework.
- `README.md`: This documentation.