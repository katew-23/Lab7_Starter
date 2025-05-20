### Intro ###
1. Within a Github action that runs whenever code is pushed. Automated tests are most effective when integrated early into the development workflow, so placing them within a GitHub action that runs on every push ensures that any new changes are immediately tested. This helps catch bugs early, maintain stability, and prevent broken code from being merged into the main branch. Running tests automatically also removes the risk of forgetting to run them manually.

### Expose ###
2. No. E2E tests are designed to simulate real user interactions with your application through the browser — like clicking buttons, filling out forms, or navigating between pages. They test the full workflow of the app, not individual functions. If you want to check whether a function returns the correct output, you should use unit tests.


