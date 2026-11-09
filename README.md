# Web template

A reusable starting point for web applications built with Vite, JavaScript, and
Tailwind CSS. Includes hot reload, code checks, and a production build.

## Requirements

- Node.js `20.19+` or `22.12+`
- npm

## Getting started

1. Use this folder as a template or copy its files into your new project.
2. Change the `name` field in `package.json` to your project name (lowercase,
   hyphen-separated, with no spaces).
3. Update the page title and description in `index.html`.
4. Install dependencies and start the development server:

   ```bash
   npm install
   npm run dev
   ```

5. Open the URL shown in the terminal (by default,
   [http://localhost:5173](http://localhost:5173)).

Tailwind CSS is configured with the official Vite plugin. Use utility classes
in `src/main.js` and add custom styles in `src/style.css`.

## Push to GitHub

1. Create an empty GitHub repository and use `main` as its default branch.
2. If this folder is not already a Git repository, run these commands from the
   project folder (replace `<USERNAME>` and `<REPOSITORY>`):

   ```bash
   git init
   git add .
   git commit -m "Initial project setup"
   git branch -M main
   git remote add origin https://github.com/<USERNAME>/<REPOSITORY>.git
   git push -u origin main
   ```

To build the production site locally, run `npm run build`. The generated files
are written to `dist/`.

## Available commands

| Command                | Description                                            |
| ---------------------- | ------------------------------------------------------ |
| `npm run dev`          | Starts the development server with hot reload.         |
| `npm run lint`         | Lints JavaScript, CSS, JSON, and Markdown with ESLint. |
| `npm run format`       | Formats files with Prettier.                           |
| `npm run format:check` | Checks formatting without changing files.              |
| `npm run build`        | Creates the production files in `dist/`.               |
| `npm run preview`      | Serves the build locally. Run `npm run build` first.   |
| `npm run check`        | Runs formatting checks, lint, and build.               |

## Project structure

```text
.
├── index.html
├── public/
│   └── favicon.svg
├── src/
│   ├── main.js
│   └── style.css
├── eslint.config.js
├── vite.config.js
├── package.json
└── package-lock.json
```

To add local environment variables, create a `.env.local` file (already ignored
by Git). Variables exposed to the browser must start with `VITE_`. Never put
secrets in them: their values are included in the code sent to the browser.
