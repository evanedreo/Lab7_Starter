1. ## Where would you fit your automated tests in your Recipe project development pipeline?

Within a GitHub Action that runs whenever code is pushed. Because it ensures that every change pushed to the repository is automatically tested. This gives immediate feedback, catches bugs early, and make sure consistent quality throughout the development process. It also supports collaboration by enforcing quality checks on pull requests, avoiding breaking changes.

2. ## Would you use an end-to-end test to check if a function is returning the correct output?

No. End-to-end tests simulate real user interactions and are best used to test entire user flows and system integration. To check if a function returns the correct output, a unit test is more useful, because it is designed to test individual functions.

3. ## What is the difference between navigation and snapshot mode?
- navigation = Lighthouse loads the whole page from the start, like a real user visiting the site. It measures how fast things show up, how stable the layout is, and how everything performs during a full page load. It’s good for testing full user experience from the moment someone lands on the page.

- snapshot = Lighthouse takes a look at the page as it is right now, without reloading it. It checks the current state of the HTML, CSS, and elements already on the screen. This is useful when we want to test a single component or view that’s already rendered.

4. ## Three things we could do to improve the CSE 110 shop site based on the Lighthouse results:
- Properly size images and serve them in next-gen formats (e.g., WebP)
This would reduce load times and improve Largest Contentful Paint (LCP), optimizing images can significantly enhance performance scores.

- Add a `<meta name="viewport">` tag
This is important for responsive design on mobile devices, it allows the page to scale properly and makes the text easier to read and the layout more consistent.

- Add missing HTML attributes for SEO and accessibility
The site is missing important tags like `<html lang="en">` and a `<meta name="description">`. These will help search engines understand the content and make the page easier to use for screen readers.





