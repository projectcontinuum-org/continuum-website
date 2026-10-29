<div align="center">
  <h1>Continuum Website</h1>
  <strong>Source of the Project Continuum website at <a href="https://projectcontinuum.org">projectcontinuum.org</a></strong>
</div>

<div align="center">
  <img src="https://img.shields.io/badge/License-Apache_2.0-green" alt="License: Apache 2.0">
  <img src="https://img.shields.io/badge/React-18-61dafb?logo=react&logoColor=white" alt="React 18">
  <img src="https://img.shields.io/badge/TypeScript-5-blue?logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Vite-6-646cff?logo=vite&logoColor=white" alt="Vite 6">
  <img src="https://img.shields.io/badge/Tailwind_CSS-3-38bdf8?logo=tailwindcss&logoColor=white" alt="Tailwind CSS 3">
</div>

---

## Part of Project Continuum

This is the marketing and introduction site for [Project Continuum](https://github.com/projectcontinuum-org), an open-source, cloud-native, no-code workflow platform. Product documentation lives in [continuum-docs](https://github.com/projectcontinuum-org/continuum-docs) at [docs.projectcontinuum.org](https://docs.projectcontinuum.org).

## Tech stack

- [React](https://react.dev/) 18 and [React Router](https://reactrouter.com/)
- [Vite](https://vitejs.dev/) and TypeScript
- [Tailwind CSS](https://tailwindcss.com/)
- [Framer Motion](https://www.framer.com/motion/) for animation
- [React Flow](https://reactflow.dev/) (`@xyflow/react`) for the workflow preview

## Quick start

You need **Node.js 20 or later** (CI uses Node 22).

```bash
git clone https://github.com/projectcontinuum-org/continuum-website.git
cd continuum-website
npm install
npm run dev
```

| Command | What it does |
|---|---|
| `npm run dev` | Start the Vite dev server |
| `npm run build` | Type-check and build to `dist/` |
| `npm run preview` | Serve the production build locally |

## Project layout

```
src/
  App.tsx            Routes and page layout
  components/        Hero, Features, SneakPeek, WorkflowPreview, Footer
  index.css          Tailwind entry point
public/              Logo, favicon and static assets
```

## Deployment

Every push to `main` runs the [deploy workflow](.github/workflows/deploy.yml), which builds the site and publishes it to the `gh-pages` branch for GitHub Pages, served on `projectcontinuum.org`. Pull requests run a build check ([pr-check workflow](.github/workflows/pr-check.yml)).

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) and the organization's [Code of Conduct](https://github.com/projectcontinuum-org/.github/blob/main/CODE_OF_CONDUCT.md).

## License

[Apache 2.0](LICENSE)
