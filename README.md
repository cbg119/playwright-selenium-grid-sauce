# playwright-selenium-grid-sauce
Repository to host examples of using Playwright's Selenium Grid feature to run tests on Sauce Labs
- https://playwright.dev/dotnet/docs/selenium-grid
- https://docs.saucelabs.com/web-apps/automated-testing/playwright/selenium-grid/

## Node Setup

1. Clone directory
2. Navigate to directory
3. Run `npm i`
4. Run the following command, ensuring to use your own Sauce Labs username and access key:
```
SELENIUM_REMOTE_URL=https://ondemand.us-west-1.saucelabs.com:443/wd/hub \
SELENIUM_REMOTE_CAPABILITIES='{"platformName":"Windows 11","browserName":"chrome","sauce:options":{"devTools":true,"username":"your_user","accessKey":"your_access_key"}}' \
npx playwright test --headed
```