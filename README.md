# learning-react

* We have set components that are injected into DOM.
* A **virtual DOM** is created with these components that is later updated in browser dom.
* State for virtual DOM is maintained and browser dom is refreshed/updated when component state changes.
* A component is JSX(Java Script XMl)
  * state (data or UI state for that component)
  * java script for functionality.
* 
  * Code editor - https://code.visualstudio.com/
  * GitHub repository (course files) -  https://github.com/iamshaunjp/react-r...
  * React CDN - https://reactjs.org/docs/cdn-links.html
##### Visual Studio Code useful extensions
  * HTML5 Boilerplate
  * ES7 React/Redux/GraphQL/React-Native snippets
  * Live Server
  * Monokai++
  * Sublime Babel
##### Chrome extension
* https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en
  
#### Components
* A react application is made of components.
###### Component types
* class based components (extends React.Component)
   * Each component has state and return a behaviour of an element through **render** method.
   * The element can have inner elements, but there will be only one element at root level.
   * we can't use **class** in JSX in components, instead we use className.
##### Useful links
   * https://reactjs.org/docs/events.html#supported-events
   * https://medium.freecodecamp.org/this-is-why-we-need-to-bind-event-handlers-in-class-components-in-react-f7ea1a6f93eb
#####  Create React App (command line tool to generate react project )
* https://github.com/facebook/create-react-app

##### About React
* React apps are typically single page applications.
* Only ever one HTML served to browser.
* React then controls what user see on the page.
* Is made of components.
 * A component can has sub comonents... like a Java class have object references.
 * A component can pass properties to sub components. through key=value
   * https://github.com/neerajmahajan/react-redux-complete-playlist/tree/lesson-13/myapp/src
 * We can also pass **list of objects** to a sub component.
   * https://github.com/neerajmahajan/react-redux-complete-playlist/tree/lesson-14/myapp
##### Component Types
* Container Components or Class based components
   * Contain state.
   * Contain lifecycle hooks.
   * Not Concerned with UI.
   * Use classes to create.

* UI Components or Stateless Components - https://github.com/neerajmahajan/react-redux-complete-playlist/blob/lesson-14/myapp/src/Ninjas.js
   * Don't contain state.
   * Recieve data from props.
   * Only concerned with UI.
   * Use functions to create.
* Map function is used to return a list + Conditional output
  * https://github.com/neerajmahajan/react-redux-complete-playlist/blob/lesson-16/myapp/src/Ninjas.js
* Taking inputs from form and passing to other components.
  * https://github.com/neerajmahajan/react-redux-complete-playlist/blob/lesson-17/myapp/src/AddNinja.js
* Passing functions as props to a component and updating master component state through that function.
  * https://github.com/neerajmahajan/react-redux-complete-playlist/blob/lesson-18/myapp/src/App.js
  * Spread Operator
   * let ninjas = [..this.state.ninjas, ninja]
   * ... add add elements of existing array to a new array
   * delete https://github.com/neerajmahajan/react-redux-complete-playlist/blob/lesson-19/myapp/src/App.js
 ##### React Lifecycle https://github.com/neerajmahajan/react-redux-complete-playlist/blob/lesson-22/myapp/src/App.js
 * http://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/
 * Mounting
  * constructor - Usually used to set the state of component.
  * getDerivedStateFromProps
     * Is called when the component is going to rendered first time.
     * when the passed parameters to the components are changed.
  * render (in virtual DOM)
  * React update DOM and references
  * componentDidMount : fires after component mount. Can load data from database
 * Updating
  * getDerivedStateFromProps
  * shouldComponentUpdate : check new props and old props
  * render
  * getSnapshotBeforeUpdate (Read only access to real DOM)
  * React Update DOM and references
  * componentDidUpdate
 * Unmounting
  * componentWillUnmount
   
