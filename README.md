The fastest way to hit the ground running with React for your next [Mintbean](https://www.mintbean.io/) challenge!

Comes with `gh-pages` to deploy your React app without the fuss. 

## Get started
### Install `create-react-app`
```
 yarn global add create-react-app
 ```
 or 
 ```
 npm install -g create-react-app
 ```

### Create new React app with template
Replace `<my-app>` with your new app name
```
create-react-app <my-app> --template cra-template-mintbean-challenge-react-starter
```

### Create new github repo for your project
`cd` into your new project and push it to a new Github repo using `hub` (don't have `hub`? [install it](https://github.com/github/hub#installation) )
```
git add .
git commit -m "init"
hub create
git push origin master
```
A new repo has been created in your Github with the name of your project. Get coding! 

## Deploy to Github Pages 
Deploy your app at any time after setting up the following config. 

### 1. Update `package.json`
**IMPORTANT** In `package.json`, between the "name" and "version" keys, add a new key "homepage". Replace values with your `<github-username>` and `<repo-name>`
```
{ 
  ...
  "homepage": "https://<github-username>.io/<repo-name>/",
  ...
}
```

### 2. Deploy
Push any updates you have to master, then run: 
```
yarn deploy
```
or if you use npm:
```
npm run deploy
```

That's it! You're app is now publically demo-able at `https://<github-username>.io/<repo-name>/`

### Note
By default, Github pages builds off `master` branch, so push any changes you want deployed there. 

If you can't find your Github Page, go to your repo > "Settings" > scroll to Github Pages section. 

-----------------------------------------
-----------------------------------------
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `yarn build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
