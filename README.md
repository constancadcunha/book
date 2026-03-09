# Folio & Co.

A simple bookshop app built for UX evaluation. There are two versions: one that works properly (this one) and one that's deliberately broken with 18 usability bugs.

- Root directory: clean, working version
- `buggy/` directory: broken version for testing

## Running it

Just open `index.html` (or `buggy/index.html`) in a browser. No server needed. Cart data saves to localStorage.

To clear the cart: open console and run `localStorage.clear()`

## What it's for

This is for comparing UX evaluation methods on the same interface. The study uses three approaches:
- Heuristic evaluation (Nielsen's heuristics)
- Task analysis (completion rates, time, errors)
- Self-assessment manikin (emotional response)

Participants try to complete 5 tasks:
1. Find a book by searching for the author's name
2. Filter books by the "Science" genre
3. Add two books to cart
4. Remove one specific book from cart
5. Complete checkout

## Files

Clean version (root):
- 4 HTML pages
- 1 CSS file
- 5 JS files (`books-data.js`, `books.js`, `cart.js`, `cart-page.js`, `checkout.js`)

Buggy version (`buggy/`):
- Same structure
- Plus `BUGS.md`, `COMPARISON.md`, and `CHECKLIST.md`

Only `books-data.js` is identical between versions.

## Tech stack

Plain HTML, CSS, and JavaScript. No frameworks. Uses localStorage for the cart.
