# Cucumber with JS
Special credits for [`nightwatch-cucumber`](https://github.com/mucsi96/nightwatch-cucumber)
## How to Use


### Installation
```
npm i -g ntl
git clone git@github.com:fathirwafda/pirate-ship.git
cd pirate-ship
npm i

```
### Execute the test (choose ntl or npm)
ntl
```
npm task list:
ntl  -> then choose one of the tasks from the list
```
npm
```
Single feature file:
npm run e2e-test -- features/feature_file.feature
or
npm run e2e-test -- features/feature_file

Multiple feature files:
npm run e2e-test -- features/feature1_file features/feature2_file

Single scenario by its line number:
npm run e2e-test -- features/feature1_file.feature:5

Scenario tags:
npm run e2e-test -- --tag tag_name
```

## Troubleshooting
If you already have chromedriver installed (via Homebrew, for example), then you may see an error when installing chromedriver with `npm install`. You can point
`webdriver.chrome.driver` in the config file to your chromedriver path (**/usr/local/bin/chromedriver**).
Make sure to comment out `const chromedriver = require('chromedriver');`    if you do this.
