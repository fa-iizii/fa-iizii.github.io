# Portfolio Website

Personal developer portfolio and interactive resume, built as a lightweight static site. The visual design and interactions live in `index.html`, while `portfolio.json` holds the information displayed on the page.

**Live site:** [fa-iizii.github.io](https://fa-iizii.github.io) · [fa3z.com](https://fa3z.com)

## Key Features

- **Dot-matrix background:** Canvas animation responds to pointer movement and clicks.
- **Glass-style interface:** Translucent cards sit over the animated background.
- **Motion and scrolling:** GSAP, ScrollTrigger and Lenis handle page animations and smooth scrolling.
- **Interactive details:** Includes a Snake game and a text-scramble effect.
- **Responsive layout:** Sections and project cards adapt to different screen sizes.
- **Separate portfolio content:** Update the JSON file to change the displayed information without editing the page layout.

## Technical Stack

- **Markup, styling and application code:** HTML5, CSS3 and vanilla JavaScript in `index.html`
- **Background:** HTML Canvas API
- **Animation:** GSAP, ScrollTrigger and Lenis
- **Content:** JSON loaded by the browser with `fetch()`
- **Hosting:** GitHub Pages

## How the JSON Content Works

When the page loads, JavaScript fetches `portfolio.json` and uses its data to fill in the profile, projects, experience, education, certifications, journey and stats sections. The design stays in `index.html`; the text and entries stay in the JSON file.

To update the portfolio, edit the relevant section in `portfolio.json`. To add an item, copy an existing item in that section and change its values. Keep the same field names and valid JSON syntax: use double quotes and commas between fields and items, with no comma after the final item. A JSON validator can help catch syntax mistakes.

Project images use paths such as `images/campus.png`. Keep each image in the `images` folder and use its correct filename in the JSON. Only include information you want to make public.

## Project Structure

```text
/
├── index.html       # Layout, styles and JavaScript
├── portfolio.json   # Text and portfolio entries
├── README.md        # Project notes
└── images/          # Project images
```

## Run Locally

Because the page loads `portfolio.json`, run it through a local web server instead of opening `index.html` directly.

```bash
python3 -m http.server 8000
```

On Windows, you can use `py -m http.server 8000`. Then open <http://localhost:8000>. Press Ctrl+C in the terminal to stop the server.

## Publish

Commit and push changes to the GitHub repository. GitHub Pages serves the static files; there is no build step. Keep `index.html`, `portfolio.json` and the `images` folder in the published directory. Fonts and animation libraries are loaded from public CDNs.

Designed and developed by Faiz Muhammed.
