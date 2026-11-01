# Assignment 8.5 - CSS Grid Mini-Project

## GitHub Link

https://github.com/udaypratapsingh007/Assignment-8.5

## Description

A responsive photo gallery website built with CSS Grid. It has a header, a main gallery grid with eight photos, consistent gaps and a footer.

## Grid Usage

- Primary layout: the .page container uses display: grid with grid-template-areas for the header, main and footer, so each section has a named grid area.
- Gallery: the .gallery container uses grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)). Each column is at least 220px wide and shares the free space with the fr unit, so the number of columns changes automatically with the screen width.
- Gaps: one gap variable (15px) is used for all the spacing, so the gaps are consistent.
- Explicit placement: the featured photo uses grid-column: span 2 and grid-row: span 2, so it is larger than the other photos.

## Preventing Overflow

Images use width: 100%, height: 100% and object-fit: cover, so they fill their box without stretching or overflowing. The heading uses overflow-wrap: break-word, and the photo boxes use overflow: hidden.

## Responsive Test

I tested the page at different widths using the device toolbar in Chrome DevTools. The number of columns reduces as the screen gets smaller, and on narrow screens the featured photo changes to a normal size.

Desktop width:

![Desktop view](desktop.png)

Mobile width:

![Mobile view](mobile.png)