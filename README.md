# React-Tutorial

### Quick Start
- [X] https://reactjs.org/docs/installation.html#creating-a-new-application

# React Tutorial CommentBox
- [X] https://medium.com/@gsuppy/coding-an-interactive-comment-box-with-react-js-50d7d20587d8
  ## Quick Start Tutorial: React Redux
  - [ ] https://medium.com/@firasd/quick-start-tutorial-using-redux-in-react-apps-89b142d6c5c1
  ## Quick Start Tutorial: Universal React, with Server Side Rendering 
  - [ ] https://medium.com/@firasd/quick-start-tutorial-universal-react-with-server-side-rendering-76fe5363d6e

# Real time twitter Stream: 
- [ ] https://scotch.io/tutorials/build-a-real-time-twitter-stream-with-node-and-react-js

# Getting to know Flux: 
- [ ] https://scotch.io/tutorials/getting-to-know-flux-the-react-js-architecture



# Handling 'this', how to bind to method 
- [X] https://reactjs.org/blog/2015/01/27/react-v0.13.0-beta-1.html#autobinding


# Create React App with an Express Backend 
- [ ] https://daveceddia.com/create-react-app-express-backend/


# Setup React without `create-react-app` from scratch
- [x] https://medium.com/@robhitt/react-from-scratch-575d1e570b85
  ## Implementing redux and react-router v4 in your react app
- [ ] http://manojsinghnegi.com/blog/2017/09/03/Implementing-redux-and-react-router-v4-in-your-react-app/


# Using React with Webpack
https://blog.risingstack.com/using-react-with-webpack-tutorial/




Whenever `this.setState` is called, an update to the component is scheduled, causing React to merge in the passed state update and rerender the component along with its descendants.

 - NEVER mutate `this.state` directly, as calling `setState()` afterwards may replace the mutation you made. Treat this.state as if it were immutable.

 - `setState()` does not immediately mutate this.state but creates a pending state transition. Accessing `this.state` after calling this method can potentially return the existing value.

 - There is no guarantee of synchronous operation of calls to setState and calls may be batched for performance gains.  `setState()` will always trigger a re-render unless conditional rendering logic is implemented in `shouldComponentUpdate()`.

 - If mutable objects are being used and the logic cannot be implemented in `shouldComponentUpdate()`, calling `setState()` only when the new state differs from the previous state will avoid unnecessary re-renders.


`functional components` Rather than define a class extending React.Component, simply write a function that takes props and returns what should be rendered.


### Note
- JS use 2 spaces instead of tab
- It is, however, conventional in React apps to use on* names for the attributes and handle* for the handler methods.
