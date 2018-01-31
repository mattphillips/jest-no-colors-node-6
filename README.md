# jest-no-colors-node-6

When you run jest@22 in Node 6 with 20 or less test suites then any failing tests are logged with colors.

When there are more than 20 test suites colors become disabled.

To see this in action (using node 6):

```bash
# clone this repo:
git clone git@github.com:mattphillips/jest-no-colors-node-6.git

# install jest
yarn install

# run the test and see 1.test.js is failing and logs with colors enabled
yarn test

# rename 21.xtest.js to 21.test.js to make it a valid test file
mv 21.xtest.js 21.test.js

# run the tests again and see that 1.test.js is still failing but logs with no colors
yarn test
```
