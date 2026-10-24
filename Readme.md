# Task 8: CSS - Laundry Services Hamburger Menu in Mobile

Mobile hamburger menu for the laundry services page, built with plain HTML and CSS only (no Bootstrap, no JavaScript).

## Files

- `index.html` - page structure (navbar with hamburger button + hero section)
- `style.css` - styling and media queries, linked from the HTML
- `laundry.png` - laundry illustration in the hero section
- `Readme.md` - this file

## How it works

- **Hamburger icon:** three bars wrapped inside a `<button>` in the navbar. It is hidden by default (`display: none`) and shown only in mobile view (`max-width: 600px`).
- **Menu list:** a `div` with `position: absolute` on the right side of the screen. Its default is `display: none`.
- **Showing the list on click:** the button receives focus when clicked, so the CSS selector `.menu-btn:focus + .menu-list { display: block; }` shows the list. This works because the menu list is a sibling of the button. `.menu-list:focus-within` keeps the list open while a link inside it is tapped.
- **Hiding the list:** clicking anywhere else removes focus, so the list hides again.

## Responsive behaviour

| Screen | Width | Navbar |
| --- | --- | --- |
| Desktop | above 992px | Logo, links and username; no hamburger |
| Tablet | up to 992px | Smaller logo, links and username; no hamburger |
| Mobile | up to 600px | Links hidden; logo, username and hamburger icon; menu opens on the right |

## How to run

Keep `index.html`, `style.css` and `laundry.png` in the same folder and open `index.html` in a browser. Use the device toolbar (or resize the window below 600px) and click the hamburger icon.
