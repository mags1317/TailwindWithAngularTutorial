# Lesson 2: Installation and Configuration

**Duration:** 10 minutes

## Overview

In this lesson, we'll walk through the process of installing Tailwind CSS into your Angular project and configuring it to fit your project's needs.

## Installation

To install Tailwind CSS along with its dependencies, open your terminal and navigate to your Angular project directory. Then, run the following command:

```bash
npm install -D tailwindcss postcss autoprefixer
```

## Configuration

After installing Tailwind CSS and its dependencies, you'll need to initialize the Tailwind configuration file to customize the framework to fit your project's needs. To generate a default configuration file, run the following command:

```bash
npx tailwindcss init
```

This command creates a tailwind.config.js file in your project directory, which you can customize according to the Tailwind CSS documentation and your project requirements.

###`tailwind.config.js` File
The tailwind.config.js file allows you to customize Tailwind CSS's behavior and extend its functionality. Here's an example of what the configuration file might look like:

```js
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
content: Specifies the content that Tailwind CSS should scan to find where your classes are being used.
theme: Allows you to extend or customize Tailwind CSS's default theme.
plugins: Allows you to add plugins to Tailwind CSS.

###`@tailwind` At-Rules
In your CSS or SCSS files, you'll use @tailwind directives to include Tailwind's base styles, component styles, and utility classes. Here's how you would include them in your stylesheet:

```css
/* styles.css */

/* Include Tailwind's base styles */
@tailwind base;

/* Include Tailwind's component styles */
@tailwind components;

/* Include Tailwind's utility classes */
@tailwind utilities;
```

In the next lesson, we'll explore practical examples of using Tailwind CSS classes in HTML.
