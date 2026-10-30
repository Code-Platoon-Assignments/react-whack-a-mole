# React: Whack-A-Mole

### **Note:** this project was first created with `create-react-app` (React 17). It has been moved to Vite + React 19, so it works like the projects you create with `npm create vite`: the files end in `.jsx` and `npm run dev` starts the dev server. You need Node 20.19+ or 22.12+ (the devcontainer uses Node 24).

Two factors determine what a React Component renders:
  1. `Props` - properties passed into the component from its parent.
  2. `State` - the internal state of a component

If you haven't already, read the React docs on [props](https://react.dev/learn/passing-props-to-a-component) and [state](https://react.dev/learn/state-a-components-memory) to get a better sense of these two concepts.

In this challenge, we'll be building a [Whack-A-Mole](https://en.wikipedia.org/wiki/Whac-A-Mole) game. This challenge will give us more practice with using state and props values in React. 

Instead of creating a React app from scratch, we'll instead be working on an existing (pre-created) React app. Instead of running `npx create vite`, we instead will need to navigate into the project (the same level as the `package.json` file) folder and run `npm install`. NPM will look at our `package.json` file and install all the required libraries for this project. (This is akin to running `pip install -r requirements.txt` for Django projects)

```sh
cd react-whack-a-mole
npm install
npm run dev
```

Then open [http://localhost:5173](http://localhost:5173) in your browser.

The game "engine" has already been created. The state variable of the top-level component, `App.jsx`, contains two items:
  1. **dens** - an array of objects that are a representation of the "holes" in the whack-a-mole game.
  2. **points** - an integer that contains the number of times a mole was whacked/clicked.

Inspect `App.jsx` and attempt to understand the game engine logic. It may take some time to understand all the connections, but this is our job as a developer to figure out how everything here should work.

## Release 0
- Modify the `props` that are passed into the `Mole.jsx` component itself so that the Mole image only appears when the **isMoleVisible** property of the appropriate **den** object is set to true.

## Release 1
- Modify `Mole.jsx` so that points are incremented whenever a visible mole is clicked.
- Add comments to the `startGame()`, `getDensState()`, and `onMoleWhacked()` functions that explain what the code is doing.


