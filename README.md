# Corvelle

Public site and support hub for **Corvelle** - a native iPhone app for chatting
with an AI assistant you host on your own server. Approve what the assistant
does, share your reminders and calendar only when you choose, and keep your
data on infrastructure you control.

## Links

- **Privacy policy:** https://tarakanof.github.io/Corvelle-Site/privacy/
- **Support:** https://tarakanof.github.io/Corvelle-Site/support/ - email
  <corvelle@akitaka.me>, or [open an issue](https://github.com/tarakanof/Corvelle-Site/issues)
  (bug reports, questions, and feature requests welcome)
- **Marketing page:** https://tarakanof.github.io/Corvelle-Site/

## Privacy in one line

The developer collects no data: no accounts, no analytics, no tracking. The app
talks only to the server you pair it with. See the
[full policy](https://tarakanof.github.io/Corvelle-Site/privacy/).

---

This repository hosts the static site served at
https://tarakanof.github.io/Corvelle-Site/ via GitHub Pages. The app itself is
developed in a separate private repository.

The site is built with [Astro](https://astro.build): pages live in
`src/pages/`, the shared layout in `src/layouts/Base.astro`. Pushing to
`main` builds and deploys via `.github/workflows/deploy.yml`. Local dev:
`npm install && npm run dev`.

`npm run check` is the pre-merge gate: `astro build`, then an internal-link
check over `dist/`.
