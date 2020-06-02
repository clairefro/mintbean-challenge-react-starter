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

### Create a new Github repo 
`cd` into your new project and push it to a new Github repo using `hub create` 
(don't have `hub`? [install it](https://github.com/github/hub#installation) )
```
git add .
git commit -m "init"
hub create
git push origin master
```
A new repo has been created in your Github with the name of your project. 

Run `yarn start` to start your dev server. Get coding! 

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
By default, Github pages builds off `master` branch, so push any changes you want deployed there. You can run `yarn deploy` as often as you like. Be sure to deploy one last time at the end of the proejct period! 

### Where's my page???
If you can't find your Github Page, go to your repo > "Settings" > scroll to Github Pages section. 

-----------------------------------------
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).
