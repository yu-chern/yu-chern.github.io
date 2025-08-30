
# Project Overview

This is a personal portfolio website built with [Astro](https://astro.build/) and styled with [TailwindCSS](https://tailwindcss.com/) and [DaisyUI](https://daisyui.com/). The website includes a blog, a curriculum vitae (CV) section, a project showcase, a store, and an RSS feed.

The project is structured as a typical Astro project, with most of the source code located in the `src` directory.

-   **`src/components`**: Contains reusable Astro components for building the website's user interface.
-   **`src/content`**: Manages the website's content, including blog posts and store items, using Astro's content collections feature.
-   **`src/layouts`**: Defines the overall structure and layout of the website's pages.
-   **`src/pages`**: Contains the individual pages of the website, with some pages being generated dynamically from the content collections.
-   **`src/styles`**: Holds the global CSS styles for the website.
-   **`public`**: Stores static assets like images and the `robots.txt` file.

# Building and Running

To work with this project, you need to have [pnpm](https://pnpm.io/) installed.

**Installation:**

To install the project's dependencies, run the following command in your terminal:

```bash
pnpm install
```

**Running the Development Server:**

To start the local development server, use the following command:

```bash
pnpm run dev
```

This will launch a development server, allowing you to view the website in your browser and see your changes update live.

**Building for Production:**

To build a production-ready version of the website, run this command:

```bash
pnpm run build
```

This will create an optimized version of the website in the `dist` directory, which can then be deployed to a web server.

# Development Conventions

-   **Styling**: The project uses TailwindCSS for utility-first styling and DaisyUI for pre-built UI components. Custom styles can be added to the `src/styles/global.css` file.
-   **Content**: Blog posts and store items are written in Markdown and managed as content collections in the `src/content` directory. The schema for these collections is defined in `src/content/config.ts`.
-   **Components**: The website is built using reusable Astro components, which can be found in the `src/components` directory.
-   **Configuration**: The main configuration for the Astro project is in `astro.config.mjs`, while the TailwindCSS configuration is in `tailwind.config.cjs`. Site-wide settings, such as the title and description, are located in `src/config.ts`.
-   **Layouts**: The overall page structure is defined by layouts in the `src/layouts` directory. The `BaseLayout.astro` file serves as the main layout for most pages.
