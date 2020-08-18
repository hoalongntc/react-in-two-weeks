# React in 2 weeks roadmap


## 1. Development environment
It’s recommended to set up a local environment for better development experience. But you can choose to use some online IDEs also: https://codesandbox.io/, https://stackblitz.com/

The local development environment requires NodeJS and npm, and an IDE of choice.

### 1.1 NodeJS and npm
You can head up to the NodeJS [download page](https://nodejs.org/en/download/) and follow the instructions to get the latest version of NodeJS.

A more preferable way to install NodeJS is to use nvm, a NodeJS version management tool.

You can follow [nvm install instructions](https://github.com/nvm-sh/nvm#install--update-script) or simply run:
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash

# or

wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```

Then install NodeJS with:
```bash
nvm install 10
# install latest NodeJS version 10
```

Check your installation with:
```bash
node -v
# v10.19.0
npm -v
# 6.13.4
```
*Note: It's ok if your version is different than my*

### 1.2 Install your IDE
You should use [VSCode](https://code.visualstudio.com/download) for development but Sublime Text, IntelliJ or any text editor can be used. 

Here are some extensions you should install to make the development better:
  - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode): Code formater
  - [React Simple Snippets](https://marketplace.visualstudio.com/items?itemName=burkeholland.simple-react-snippets): Snippets for faster React development.

## 2. Basic web knowledge

React development requires some basic knowledge in web development including HTML, CSS, and modern Javascript.

Here are some resources that can quickly help you get started with Javascript development:
  - [Javascript for beginners](https://www.youtube.com/watch?v=W6NZfCO5SIk): This video gives you the fundamentals of Javascript. 
  - [ES6 tutorial](https://www.youtube.com/watch?v=NCwa_xi0Uuc): ES6 or Ecmascript version 6 is a modern version of Javascript published in 2015. ES6 includes some new features that will be used a lot when developing modern Javascript apps.

## 3. Your first React app
The fastest way to scaffold a React app is to use an online editor with a React template or using [Create React App](https://create-react-app.dev/docs/getting-started) locally.

Create a new React app with CRA is just as simple as: 
```bash
npx create-react-app my-app
cd my-app`
npm start
```

[This video](https://www.youtube.com/watch?v=Ke90Tje7VS0&t) a good starting point to get to know React fundamentals.

## 4. Calculator App

Its time to create your own React app. Your first React app can be anything, and a calculator app is a good starting point. 

![Calculator example](https://daveceddia.com/images/calculator@2x.png)

Your app functionality should include:
  - number keypad 
  - basic math operators: add, subtract, multiply, divide
  - clear
  - advanced: capture keyboard events instead of clicking with the mouse.

This app will help you get better with React state management and events handling.
Spend a little time thinking about how the state will be represented. Do you need to store more than just the numbers on the display? When you type a new number, does it replace the display with that number, or append it to the end?

## 5. Weather App
![Weather App](https://daveceddia.com/images/weather@2x.png)

This app will help you get started with remote data loading and asynchronous action handling.

Display a 5-day weather forecast, where each day shows the high and low temperatures and an image for sunny/rainy/cloudy/snowy. Use fake, hard-coded data until you’ve got everything rendering correctly.

The next step is to sign up for a free API key from [Open Weather Map](https://openweathermap.org/), fetch a real 5-day forecast, and feed that data into your app.

Next, add the ability to click on a day, and see its hourly forecast. You can just maintain the current view in the top-level App state.

## 6. What's next?
After getting familiar with basic React concepts, it's time to dig deeper.
Here are some topics that you could choose to learn:

### 6.1 State management
https://reactjs.org/docs/faq-state.html
https://reactjs.org/docs/context.html

### 6.2 Client-side routing
https://reactrouter.com/web/example/basic

###  6.3 React hooks
https://reactjs.org/docs/hooks-intro.html

### 6.4 Error boundaries
https://reactjs.org/docs/error-boundaries.html
