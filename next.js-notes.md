# Project Initialization

## Command Used
```bash
npx create-next-app@latest nextjs-dashboard \
  --example "https://github.com/vercel/next-learn/tree/main/dashboard/starter-example" \
  --use-pnpm
```

# Next.js Routing Comparison: App Router vs Pages Router

---

## App Router (`app/`)

- Modern routing system in Next.js
- Server Components by default
- Supports nested layouts and layout persistence
- Enables streaming and progressive rendering
- Supports Route Handlers and Server Actions
- Used by the official Next.js dashboard tutorial
- Recommended for new projects

---

## Pages Router (`pages/`)

- Legacy / classic routing system
- Client Components by default
- Uses `getServerSideProps`, `getStaticProps`, `getInitialProps`
- Simpler and more explicit data-fetching model
- Large ecosystem of existing examples and patterns
- Suitable for older codebases or incremental migration

---
# CSS Modules in Next.js
---
**Reference**: [CSS modules docs](https://nextjs.org/docs/app/getting-started/css)

## Definition

- CSS Modules provide **locally scoped CSS**
- Class names are automatically namespaced
- Prevent global style collisions
- Supported natively by Next.js

---

## File Naming

- Files must be named using:
  - `*.module.css`
  - `*.module.scss`

Only files with `.module.` are treated as CSS Modules.

---

## Basic Usage

### CSS Module
```css
/* Button.module.css */
.button {
  padding: 8px 12px;
  border-radius: 6px;
}

