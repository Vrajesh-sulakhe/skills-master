---
name: bootstrap-all-rounder
description: Master unified guide and dispatcher for all Bootstrap 6 styling, component design, JavaScript plugins, migrations, bundler integration, and utility APIs. Use whenever building, styling, configuring, or migrating Bootstrap applications.
---

# Bootstrap All-Rounder

The single entry point and unified router for all Bootstrap 6 engineering tasks. Whether creating custom components, configuring color themes, wiring JavaScript plugins, migrating legacy versions, or bundling with modern build tools, this skill routes directly to the specialized Bootstrap submodule.

## When to Use This Skill
- Building or styling any Bootstrap 6 interface, layout, or component.
- Customizing colors, CSS custom properties, Sass maps, or dark mode themes.
- Implementing interactive Bootstrap JavaScript/TypeScript plugins.
- Migrating projects from Bootstrap 4 or 5 to Bootstrap 6.
- Bundling Bootstrap with Vite, Webpack, Parcel, or raw npm CLI scripts.
- Extending or authoring utilities with the Bootstrap Sass Utility API.

---

## Unified Bootstrap Routing Matrix

Read the target `SKILL.md` using `read_file` based on your specific task:

### 1. Component Authoring & UI Styling
- **CSS & HTML Structure**: [`bootstrap-component`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-component/SKILL.md)
  *Use for:* Authoring component markup, CSS custom property token maps (`$<name>-tokens`), `@layer components` cascade rules, and accessibility.
- **Interactive Plugins & Behavior**: [`bootstrap-component-js`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-component-js/SKILL.md)
  *Use for:* Writing JavaScript/TypeScript component plugins, EventHandler integration, config schemas, and event hooks.
- **Color Palette & Theme Modes**: [`bootstrap-color-system`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-color-system/SKILL.md)
  *Use for:* Sass color maps, CSS custom properties, `$theme-colors`, light/dark color modes, and WCAG contrast compliance.
- **Custom Utilities**: [`bootstrap-utility-api`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-utility-api/SKILL.md)
  *Use for:* Generating utility classes with the Sass Utility API (`$utilities`), responsive variants, and custom CSS variables.

### 2. Migration & Upgrades
- **Migrate from Bootstrap 5 to 6**: [`bootstrap-v5-v6-migration`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-v5-v6-migration/SKILL.md)
  *Use for:* Upgrading v5 codebases to v6 (cascade layers `@layer`, CSS custom property namespaces, dropping deprecated classes).
- **Migrate from Bootstrap 4 to 6**: [`bootstrap-v4-v6-migration`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-v4-v6-migration/SKILL.md)
  *Use for:* Two-major upgrade paths, handling jQuery removal, Popper upgrades, and grid changes.

### 3. Tooling, Bundlers & Installation
- **Bootstrap 6 Installation**: [`bootstrap-v6-install`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-v6-install/SKILL.md)
  *Use for:* Package manager installation (npm, yarn, pnpm) or CDN quickstart configurations.
- **Vite Setup & Bundling**: [`bootstrap-vite`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-vite/SKILL.md)
  *Use for:* Configuring `vite.config.js`, Sass resolution, Autoprefixer, and JS chunk splitting.
- **Webpack Setup & Bundling**: [`bootstrap-webpack`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-webpack/SKILL.md)
  *Use for:* Webpack loaders (`sass-loader`, `postcss-loader`), purgecss, and production minimization.
- **Parcel Setup**: [`bootstrap-parcel`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-parcel/SKILL.md)
  *Use for:* Zero-config Parcel bundling with Bootstrap Sass.
- **Raw NPM Scripts (No Bundler)**: [`bootstrap-npm`](file:///Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-npm/SKILL.md)
  *Use for:* Lightweight setups compiling Sass and JS using command-line tools without a bundler.

---

## Global Paths Quick Reference

| Sub-Skill Name | Global Path |
| :--- | :--- |
| `bootstrap-component` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-component/SKILL.md` |
| `bootstrap-component-js` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-component-js/SKILL.md` |
| `bootstrap-color-system` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-color-system/SKILL.md` |
| `bootstrap-utility-api` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-utility-api/SKILL.md` |
| `bootstrap-v6-install` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-v6-install/SKILL.md` |
| `bootstrap-v5-v6-migration` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-v5-v6-migration/SKILL.md` |
| `bootstrap-v4-v6-migration` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-v4-v6-migration/SKILL.md` |
| `bootstrap-vite` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-vite/SKILL.md` |
| `bootstrap-webpack` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-webpack/SKILL.md` |
| `bootstrap-parcel` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-parcel/SKILL.md` |
| `bootstrap-npm` | `/Users/vrajeshsulakhe/.gemini/config/skills/bootstrap-npm/SKILL.md` |

---

## Execution Workflow
1. **Analyze Intent**: Pinpoint the precise Bootstrap area needed (component, theme, utility, bundler, or migration).
2. **Read Sub-Skill**: Call `read_file` on the corresponding global path from the table above.
3. **Execute Strictly**: Implement according to the chosen sub-skill workflow and validation steps.
