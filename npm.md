Updating package in npm

npm version patch
git add *;
git commit -m "Commit message"
git push
git push --tags
npm publish

-or just after a push-
npm version patch
git push --tags  (if push command isn't set to push by default to master, then you have to explicitly git push origin master --tags)
npm publish

Bower automatically detects new versions of your package based on Git tags. Super smart and makes publishing updated packages to Bower seamless.

Update package.json dependencies to their latest versions
```js
npm i -g npm-check-updates
npm-check-updates -u
npm install
```
-------------------

### Error: Cannot find module './command'
- Delete the `node_modules` directory
- run `npm install`
