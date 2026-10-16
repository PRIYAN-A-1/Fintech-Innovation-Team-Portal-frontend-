# Prathyusha · FinTech Innovation Team

React 19 + TypeScript + Vite frontend based on the five screens in the provided Figma node `217:1882`.

## Included routes

- `/#/home` public landing page
- `/#/apply` membership application with inline validation and saved draft
- `/#/status` application status and clarification demo
- `/#/overview` student dashboard
- `/#/profile` editable profile and privacy permissions
- Extra navigation demos: projects, contributions, weekly updates, hackathons, magazine, notifications and history.

## Run on your computer

Requirements: Node.js 20.19+ or 22.12+.

```bash
npm install
npm run dev
```

Open `http://localhost:5173`. To check production compilation:

```bash
npm run build
npm run preview
```

## Important handoff notes

- This is a **functional frontend demo**, NOT a backend-connected application. Form state, profile, local edits and notifications are stored in **browser localStorage**. Nothing is sent to a server or email account. Don't use localStorage for sensitive personal data in production. Replace it with authenticated and secure APIs before real users.
- The Figma file explicitly uses **illustrative/sample records**; shown statistics are demo data.
- The college emblem at the top is a CSS/text fallback, because the Figma-provided image asset URL was not reachable from the artifact build environment. To make the logo pixel-exact, export the official logo layer (Figma node `217:1885` / `217:2217`) to `src/assets/prathyusha-logo.png`, then replace the `Logo` component in `src/App.tsx` with an `<img>` referencing it. Do not treat this placeholder as the college's official logo.
- Fonts use Manrope via Google Fonts, with system fallbacks. Offline use requires locally licensed fonts.
- Application review, account approval, notifications, uploads and login need backend APIs (and authentication), which are intentionally not simulated as completed server actions.

## Screens + Figma reference

Figma design: https://www.figma.com/design/Lr3p1WlqpWXgVklhNV3f9Z/Prathyusha-%E2%80%A2-FinTech-demo-1?node-id=217-1882

Colors: `#890C25` maroon, `#351321` dark, `#FAF7F2` cream, `#E9BE72` gold, `#E7DFDA` border.
"# Fintech-Innovation-Team-Portal-frontend-" 
