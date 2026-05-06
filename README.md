<img src="img/me-logo.svg" alt="ME monogram logo" width="100">

# About Me — Misha Evans

[![Netlify Status](https://api.netlify.com/api/v1/badges/935da2ec-0127-4cc2-89aa-cf2e82aa6a96/deploy-status)](https://app.netlify.com/projects/about-me-mknubsgit-1/deploys)

This is my About Me site for IDMX-225 at RVCC. I built it over the semester to learn HTML and CSS.

Live site: https://about-me-mknubsgit-1.netlify.app

## Description

It's a single-page site. I added a section every week or two, so it's essentially a demo of what we learned in the course.

An overview of what I picked up where:

- **Nav bar:** `<header>` and `<nav>`, flexbox, anchor links to fragments on page, smooth scroll, hover transitions on links. Stacks on phones and side-by-side at 600px.
- **Hero / Bio / Hobbies:** basic sectioning, the avatar, and a CSS grid for the hobbies list that switches from one column to 2.
- **Gallery:** `<figure>` and `<figcaption>` border around the entire thing, plus images that fill the container.
- **Blog:** drop caps using `::first-letter`. Contains a Dracula excerpt that is getting swapped out on final submit.  ## EDIT THIS BEFORE PUSHING FINAL SUBMIT ##
- **Video:** YouTube embed in an `aspect-ratio` container.
- **Contact form:** labels, fieldsets, focus states, and Netlify's form handling linked.

Netlify redeploys whenever I push to `main` without [skip netlify]

## Nav Bar

The nav bar at the top has the logo on the left and four anchor links (Bio, Gallery, Blog, Contact Me) that jump to those sections on the page using fragment IDs and `scroll-behavior: smooth`.

Below 600px wide, the link list collapses behind a hamburger icon. The toggle is pure CSS, no JavaScript. There's a hidden `<input type="checkbox">` inside the navbar, and the visible hamburger is a `<label>` for that checkbox. Clicking the label flips the checkbox state, and a `:checked ~ .navbar-links` selector reveals the menu. The three bars also morph into an X via CSS transforms when checked.

At 600px and up, the hamburger hides and the links go back to a horizontal row.

## Color Scheme

|        | Hex       | RGB                   | Locations                                  |
|--------|-----------|-----------------------|--------------------------------------------|
| ![](https://placehold.co/30x30/2A4810/2A4810.png) | `#2A4810` | `rgb(42, 72, 16)`    | Navbar background                          |
| ![](https://placehold.co/30x30/1A2210/1A2210.png) | `#1A2210` | `rgb(26, 34, 16)`    | Body text, borders, submit button          |
| ![](https://placehold.co/30x30/3F5236/3F5236.png) | `#3F5236` | `rgb(63, 82, 54)`    | Submit button hover                        |
| ![](https://placehold.co/30x30/5A6B53/5A6B53.png) | `#5A6B53` | `rgb(90, 107, 83)`   | Video caption                              |
| ![](https://placehold.co/30x30/7A9477/7A9477.png) | `#7A9477` | `rgb(122, 148, 119)` | Hero, contact form, footer, nav-link hover |
| ![](https://placehold.co/30x30/C8D2B5/C8D2B5.png) | `#C8D2B5` | `rgb(200, 210, 181)` | Hobbies block                              |
| ![](https://placehold.co/30x30/F4F1E9/F4F1E9.png) | `#F4F1E9` | `rgb(244, 241, 233)` | Page background                            |

## Citations

The writing, the photos in the gallery, and the YouTube clip are all supplied by Misha Evans (me!). The things that aren't made purely on my own:

- **BOB** (`img/logo-96X96.svg`)  from CodePen assets: <https://assets.codepen.io/385852/logo-96X96.svg>. Earlier placeholder logo, now replaced by my own monogram but kept in the repo.
- **Avatar** (`img/avataaars.png`)  made with [Avataaars](https://avataaars.com/) by Pablo Stanley.
- **Fonts:** Roboto Slab (body) and Bricolage Grotesque (headings), from Google Fonts.
- **`nav.css` comment template**  adapted from a starter gist by Cynthia Teeters: <https://gist.github.com/cynthiateeters/4e8bf8cc129d057cdb3c924447253ef2>.

### Blog article references

The "How Animated SVG Works" article in the Blog section referenced these 3 sources:

- <https://en.wikipedia.org/wiki/SVG>
- <https://www.figma.com/community/plugin/980366185319754464>
- <https://www.w3schools.com/graphics/svg_animation.asp>

## License

Code (HTML and CSS) Free use.

Everything else: all rights reserved. Do not reuse.
