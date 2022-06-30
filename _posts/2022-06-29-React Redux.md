---
Layout:
Title:  "React Redux"
Date:   "2022-06-29"
Categories:
---
# introduction
React and Redux are often mentioned together, and with good reason. The developer who created Redux was a React developer who wanted to make it easier to share data across different components.

# body
Now that you know how to manage the flow of shared data with Redux, it's time to combine that knowledge with React. In the React and Redux courses, you'll build a React component and learn how to manage state locally at the component level, and throughout the entire application with Redux.
React is a view library that you provide with data, then it renders the view in an efficient, predictable way. Redux is a state management framework that you can use to simplify the management of your application's state. Typically, in a React Redux app, you create a single Redux store that manages the state of your entire app. Your React components subscribe to only the pieces of data in the store that are relevant to their role. Then, you dispatch actions directly from React components, which then trigger store updates.

Although React components can manage their own state locally, when you have a complex app, it's generally better to keep the app state in a single location with Redux. There are exceptions when individual components may have local state specific only to them. Finally, because Redux is not designed to work with React out of the box, you need to use the react-redux package. It provides a way for you to pass Redux state and dispatch to your React components as props.



# conclusion
Over the next few challenges, first, you'll create a simple React component which allows you to input new text messages. These are added to an array that's displayed in the view. This should be a nice review of what you learned in the React lessons. Next, you'll create a Redux store and actions that manage the state of the messages array. Finally, you'll use react-redux to connect the Redux store with your component, thereby extracting the local state into the Redux store.

React Redux provides its react-redux package to help accomplish these tasks.