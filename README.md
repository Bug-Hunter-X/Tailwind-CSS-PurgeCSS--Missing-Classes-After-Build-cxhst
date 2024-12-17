# Tailwind CSS PurgeCSS: Missing Classes After Build

This repository demonstrates an uncommon issue where Tailwind CSS classes are not rendered after the build process, even if they seem to be correctly defined. This is often related to PurgeCSS, a tool that removes unused CSS from your project.

## Problem
The issue is commonly seen in Next.js and Nuxt.js projects and occurs when a Tailwind class is either misspelled or located in a component that's not properly included in the build process.  This leads to the class being purged by PurgeCSS, resulting in the element being unstyled or not displaying correctly.

## Setup
1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm run dev` to start the development server (Next.js example). Observe the bug.
5. Run `npm run build` to create a production build (Next.js example). Observe the bug.

## Solution
The solution is described in the `bugSolution.js` file and involves carefully checking for typos in class names and making sure all components using the Tailwind classes are correctly imported and rendered within the application.

## Contributing
Contributions are welcome! If you have experienced this issue in a different context, or have additional solutions, please feel free to open a pull request.