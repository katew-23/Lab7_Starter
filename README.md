### Intro ###
1. Within a Github action that runs whenever code is pushed. Automated tests are most effective when integrated early into the development workflow, so placing them within a GitHub action that runs on every push ensures that any new changes are immediately tested. This helps catch bugs early, maintain stability, and prevent broken code from being merged into the main branch. Running tests automatically also removes the risk of forgetting to run them manually.

### Expose ###
2. No. E2E tests are designed to simulate real user interactions with your application through the browser — like clicking buttons, filling out forms, or navigating between pages. They test the full workflow of the app, not individual functions. If you want to check whether a function returns the correct output, you should use unit tests.

### Explore ###
3. Navigation mode measures the performance of a page during its initial load. It provides comprehensive metrics like Performance, Accessibility, Best Practices, and SEO. This mode evaluates the entire page loading experience from start to finish.
Snapshot mode analyzes the page in its current state without considering the loading process. It only shows partial metrics. The snapshot mode focuses on the current DOM state rather than evaluating the loading behavior. It's better for finding accessibility issues on a loaded page but can't analyze JavaScript performance or loading metrics.
The key difference is that navigation mode evaluates the entire loading process and user experience metrics, while snapshot mode only analyzes the current state of a page after it's already loaded.
4. .
   1. Add a proper viewport meta tag: The error "No `<meta name="viewport">` tag found" indicates the site lacks responsive design configuration. Adding this tag would make the site properly responsive on mobile devices, improving both user experience and SEO ranking.
   2. Optimize images: Several image-related issues appear in the diagnostics:
       - "Properly size images — Potential savings of 518 KiB"
       - "Preload Largest Contentful Paint image — Potential savings of 60 ms"
       - "Serve images in next-gen formats — Potential savings of 165 KiB" <br> 
    Addressing these would significantly improve performance.
   3. Add the lang attribute to the HTML element: The Lighthouse report shows the `<html>` element is missing a [lang] attribute. Implementing this with a simple change (`<html lang="en">`) would improve accessibility and internationalization support with minimal effort.
