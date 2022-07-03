
## 端到端测试

- Install Xvfb and run Cypress again.
- https://docs.cypress.io/guides/continuous-integration/introduction#Dependencies

```sh
sudo apt-get update 
sudo apt-get install libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb
npm install --save-dev cypress
npm run cy:install
npm run cy:open

```

可忽略的问题： https://github.com/cypress-io/cypress/issues/4925

### TODO

Once you are sure that the pipeline works, write another test that ensures that one can navigate from the main page to the page of a particular Pokemon, e.g. ivysaur. The test does not need to be a complex one, just check that when you navigate a link, the page has some right content, such as the string chlorophyll in the case of ivysaur.

Note also the Pokemon ablilities are written with lower case letters, the capitalization is done in CSS, so do not search eg. for Chlorophyll but chlorophyll.

Note2 that you should not try bulbasaur, for some reason the page of that particular Pokemon does not work properly...

The end result should be something like this

