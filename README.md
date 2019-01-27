# Cucumber with JS
Special credits for [`nightwatch-cucumber`](https://github.com/mucsi96/nightwatch-cucumber)
## How to Use


Installation
```
npm i -g ntl
git clone git@github.com:fathirwafda/pirate-ship.git
cd pirate-ship
npm i

```
Execute the test
```
[If prefer using npm task list]:
ntl 

[If prefer using tags]:
npm run e2e-test -- --tag test 
```

## Troubleshooting
-If you already have chromedriver installed (via Homebrew, for example)     
-then you may see an error when installing chromedriver with `npm install`. You can point
`webdriver.chrome.driver` in the config file to your chromedriver path (**/usr/local/bin/chromedriver**).
Make sure to comment out `const chromedriver = require('chromedriver');`    if you do this.