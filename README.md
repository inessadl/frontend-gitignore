# frontend-gitignore

A generic `.gitignore` for front-end JavaScript projects, built for macOS.

## What's covered

- **macOS** - `.DS_Store`, `._*` files, Spotlight and Trash folders
- **Editors** - VS Code (keeps shared settings, extensions and launch configs), JetBrains, Vim
- **Dependencies** - npm, pnpm, Yarn (including Berry / PnP)
- **Environment variables** - all `.env` files are ignored, except `.env.example` and `.env.sample`
- **Frameworks and build tools** - Next.js, Nuxt, SvelteKit, Astro, Remix / React Router, Vite, Parcel, Turborepo, Storybook
- **Deploy** - Vercel, Netlify
- **Tests** - Jest / Vitest coverage, Playwright, Cypress
- **Caches and logs** - ESLint, Stylelint, TypeScript build info, Sass, package manager logs
- **Local certificates and keys** - `*.pem`, `*.key`, `*.crt`
- **AI assistants** - Claude Code personal settings and notes (`.claude/settings.local.json`, `CLAUDE.local.md`), while shared files like `CLAUDE.md` stay committed
- **Terminal leftovers** - Git merge and patch files, `npm pack` tarballs, `nohup.out`, Node REPL history, direnv cache

## How to use

### Start a new project from this template

Click **Use this template** at the top of this page, then **Create a new repository**.

### Add it to an existing project

Run this in the project root:

```bash
curl -o .gitignore https://raw.githubusercontent.com/inessadl/frontend-gitignore/main/.gitignore
```

> **Note:** this replaces any existing `.gitignore`. To append instead, use `curl -s <url> >> .gitignore`.

### Already committed files?

`.gitignore` only affects untracked files. If something is already in the repository, remove it from the index first:

```bash
git rm -r --cached node_modules .DS_Store
git commit -m "Stop tracking ignored files"
```

## Customizing

Every section is commented, so you can remove what your project doesn't use or add your own rules at the end of the file.

## Contributing

Found something missing? Open an issue or a pull request.
