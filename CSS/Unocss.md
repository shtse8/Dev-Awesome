### UnoCSS Setup
To integrate UnoCSS, an atomic CSS engine that provides on-demand CSS utilities, into your project, follow these steps:

**Installation:**
First, install UnoCSS via npm or Yarn:
```bash
npm install -D unocss
```
or
```bash
yarn add -D unocss
```

**Configuration:**
Create an `unocss.config.js` file at the root of your project to configure UnoCSS:
```javascript
import { defineConfig } from 'unocss';

export default defineConfig({
  // UnoCSS configuration options
});
```

**Usage:**
After configuration, start using UnoCSS by adding utility classes directly in your HTML or template files. UnoCSS will generate the corresponding CSS on-demand.

**Integration with Build Tools:**
UnoCSS can be integrated with various build tools like Vite, Webpack, Rollup, etc., by using specific plugins or configurations detailed in the UnoCSS documentation.

Reference: [UnoCSS Documentation](https://github.com/unocss/unocss)
