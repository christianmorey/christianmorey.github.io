# christianmorey.github.io

Personal portfolio for **Christian Morey** — operations manager and data analytics
practitioner in Northeast Ohio, founder of Brick Lane.

Presented as an encyclopedia article, in the spirit of a Wikipedia entry.
No affiliation with wikipedia.org or the Wikimedia Foundation.

## Stack

Static HTML, CSS, and vanilla JavaScript in a single file. No build step, no
dependencies, no framework. Type is served from Google Fonts (Spectral, Source
Sans 3, IBM Plex Mono) with system fallbacks.

## Structure

    index.html    the whole site
    404.html      not-found page, same visual language
    README.md     this file

## Features

- Light and dark themes, following the visitor's system preference
- In-page search (press `/` to focus) with match highlighting
- Contents rail that tracks scroll position
- Responsive from 320px up
- Draft-mode toggle that highlights unfinished sections

## Editing

Everything lives in `index.html`. Sections are marked with HTML comments
(`<!-- ---------- PROJECTS ---------- -->`) so they're easy to find. Design
tokens — every color, typeface, and measure — are declared once at the top of
the `<style>` block under `:root`, with the dark palette immediately below.

Unfinished content is wrapped in `<span class="todo">`. The header toggle counts
and highlights them. Delete the span wrapper as you fill each one in.

## Local preview

Open `index.html` in a browser, or:

    python3 -m http.server 8000

Then visit <http://localhost:8000>.
