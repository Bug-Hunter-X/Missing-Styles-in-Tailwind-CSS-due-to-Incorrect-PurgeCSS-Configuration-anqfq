# Missing Tailwind CSS Styles Due to Incorrect Purge Configuration

This repository demonstrates a common issue encountered when using Tailwind CSS with frameworks like Next.js or Nuxt.js.  Incorrect configuration of PurgeCSS, responsible for removing unused CSS, can lead to missing styles in the final build.

**Problem:**
The `tailwind.config.js` file's `purge` (or `content`) option may incorrectly specify paths, causing PurgeCSS to miss styles used in your components, leading to missing visual elements or broken layouts.

**Solution:**
Ensure the `content` array in your `tailwind.config.js` accurately includes all the relevant file paths where you use Tailwind classes.

See `bug.js` and `bugSolution.js` for examples of problematic and corrected code, respectively.