### Remember

Answer these on your own, then compare answers as a group

1.  What is React? 
A library and another way to write JavaScript, used to create user interfaces.
- A JS library that was created by FB
- Focuses on making UI elements and has a virtual DOM
- A collection of dependencies available in building a React app.
- Uses a component-based architecture and has unidirectional data flow.

2.  What is create-react-app?
A tool that lets you save time when building react apps. 
- A tool for putting together a React app in one go
- Sets up all the tools you need (for example, initializes a git repo.)
- A development environment with auto-refresh (npm start).

3.  What is Component Based Architecture?
A way to break up a project into smaller pieces of code (modular)
- A way to easily create scalable apps
- Self-sustaining individual blocks of code (components)

4.  What is JSX?
Helps you to write HTML in react. 
- A semantic extension of JS that is like a mix of HTML/JS
- It is the syntax react uses to describe a user interface
- Transpiled into JS ultimately

5.  What is the virtual DOM?
A concept where stuff is kept in memory and then synced to the actual DOM. 
- A "mock DOM" that keeps a copy of the actual DOM 
- It drastically in some cases increases the performance site (think big site)

6.  What is unidirectional (one-way) data flow?
- Data is passed from parent to children 
- We can get around this by passing info up through events

### Understand

Discuss these questions in pairs if you have a 4-person group

7.  Summarize what happens when you run `create-react-app my-app`
It creates a platform for you to work on to build your own react app. 
- A folder is created called "my-app"
- The folder includes our boilerplate for our app
- It creates the git repo for the app AND the package.json necessary to keep track of dependencies 

8.  Explain what this code does:

```jsx
import React from "react";

const Mentor = props => (
  <div className="mentor-container">
    <h1 className={props.title === "Lead Mentor" ? "lead" : ""}>Tim Biles</h1>
    <ul>
      <li>Fort Worth, TX</li>
      <li>My email address is timbilestimbiles@gmail.com</li>
    </ul>
  </div>
);

export default Mentor;
```

9.  Explain how data is passed from a parent component to a child component.
- By using props

### Apply

Try these on your own, but work together if you start to get stuck.

10.  Use `create-react-app` to create a new React application called `student-directory`

11.  Use the code from `Mentor` above to create a new functional, stateless component called `User` with a list of friends. Hard code the list of friends, do not use state or props.

### Analyze, Evaluate, Create

Discuss these questions as a group

12. What are the benefits and drawbacks of using a tool like create-react-app?
- Benefits:
  - We can throw together a react app quickly
  - We don't install the individual pieces separately required in a react app.
  - Most of the setup (think config files, etc) is already set up
- Drawbacks
  - it could potentially install something that we don't need leading to a bigger app size

13. Compare and contrast JSX with other templating options, such as those used in Angular or Vue

14. Compare and contrast one-way data flow with two-way data binding.
- One-way = unidirectional
- Two-way = bidirectional
