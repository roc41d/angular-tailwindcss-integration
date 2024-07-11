# Install Tailwind CSS with Angular
Setting up Tailwind CSS in an Angular project.

## Install Tailwind CSS
Install `tailwindcss` via npm, and then run the init command to generate a `tailwind.config.js` file.
```
npm install -D tailwindcss postcss autoprefixer

npx tailwindcss init
```

## Configure your template paths
Add the paths to all of your template files in your `tailwind.config.js` file.
```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./src/**/*.{html,ts}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

## Add the Tailwind directives to your CSS
Add the `@tailwind` directives for each of Tailwind’s layers to your `./src/styles.css` file.
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Start using Tailwind in your project
```
<h1 class="text-3xl font-bold underline">
  Hello world!
</h1>
```

## Start your build process
Run your build process with ng serve.
```
ng serve
```
