# Campus Coding Club — CSCI390 Project (Phase 2)

A responsive front-end web application for a student coding club, built with
**ReactJS**. This is Phase 2 of the CSCI390 Web Programming project: the original
static HTML/CSS/JavaScript site from Phase 1 was rebuilt as a component-based
React single-page application while keeping the exact same design, content, and
behaviour.

## Project Description

The Campus Coding Club website is a small informational site for a student club
focused on beginner-friendly web development. It has four pages:

- **Home** — hero section and feature cards introducing the club.
- **About** — the club's mission and main activities.
- **Gallery** — student projects with interactive category filtering (All / HTML / CSS / JavaScript).
- **Contact** — a contact form with client-side validation.

The site is fully responsive and includes a collapsible mobile navigation menu.

## Technologies Used

- **ReactJS 18** — component-based UI.
- **React Router (HashRouter)** — client-side routing across the four pages.
- **Vite** — build tool and dev server.
- **CSS3** — original Phase 1 stylesheet (responsive, mobile-first media queries).
- **Git & GitHub** — version control and hosting.

## Project Structure

```
campus-coding-club/
├── index.html              # Vite HTML entry
├── package.json
├── vite.config.js          # base: "./" for static hosting
├── src/
│   ├── main.jsx            # React entry, HashRouter
│   ├── App.jsx             # Routes + shared layout
│   ├── components/
│   │   ├── Header.jsx      # Nav + mobile menu toggle
│   │   └── Footer.jsx
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── About.jsx
│   │   ├── Gallery.jsx     # state-based filtering
│   │   └── Contact.jsx     # controlled form + validation
│   └── styles/
│       └── style.css       # Phase 1 styles, preserved
└── screenshots/
```

## Setup Instructions

You need [Node.js](https://nodejs.org/) (v18 or newer) installed.

```bash
# 1. Install dependencies
npm install

# 2. Run the development server
npm run dev
# open the printed URL (e.g. http://localhost:5173)

# 3. Build for production
npm run build

# 4. Preview the production build locally
npm run preview
```

## Deployment

The project uses a relative base path (`base: "./"`) and `HashRouter`, so the
production build in `dist/` works on static hosts without extra configuration.

- **Netlify / Vercel** — connect the repo, build command `npm run build`, publish directory `dist`.
- **GitHub Pages** — push the contents of `dist/` to a `gh-pages` branch (or use a deploy action).

## Screenshots

### Home
![Home page](screenshots/home.png)

### About
![About page](screenshots/about.png)

### Gallery
![Gallery page](screenshots/gallery.png)

### Contact
![Contact page](screenshots/contact.png)

### Mobile View
![Mobile home page](screenshots/home-mobile.png)

## Author

Abedalraheem — CSCI390 Web Programming, Department of Computer Science and
Information Technology.
