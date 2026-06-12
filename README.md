# Portfolio

A dark, code-editor-themed portfolio built with [Astro](https://astro.build).
Persistent line-number gutter, "open file" tab navigation (`about.md`,
`projects.tsx`, `skills.json`, `contact.sh`), and a hero written as literal
TypeScript.

## Customize it

Everything lives in `src/pages/index.astro`:

- **Hero** — edit the `name`, `role`, `focus`, and `status` fields in the code block.
- **About** — edit the paragraphs in the `about` section.
- **Projects** — edit the `projects` array at the top of the file (name, summary, tags, repo/demo links).
- **Skills** — edit the `skills` object at the top of the file.
- **Contact** — edit the email/GitHub/LinkedIn links and add a real `resume.pdf` to `public/`.
- **Colors/fonts** — edit the CSS variables at the top of `src/styles/global.css`.

## Run locally

```bash
npm install
npm run dev
```

Visit `http://localhost:4321`.

## Build

```bash
npm run build
```

Outputs static files to `dist/`.

## Deploy to Cloudflare Pages

1. Push this project to a GitHub repo.
2. In the Cloudflare dashboard: **Workers & Pages → Create → Pages → Connect to Git**.
3. Select the repo. Cloudflare should auto-detect the Astro framework preset
   (build command `npm run build`, output directory `dist`).
4. Once deployed, go to the Pages project's **Custom domains** tab and add
   your domain — since DNS is already on Cloudflare, the record gets added
   automatically.
