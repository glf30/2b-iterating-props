# Props Exercise

![Exercise Preview](https://i.imgur.com/p3AtNe8.png)

## Exercise overview

We are going to make an archive page for a blog site that displays a list of recent articles.

## Set Up And Run A New React App
Create a new app with `npm create vite@latest`

## Install Bootstrap

4. Next let's import Bootstrap a front-end framework that provides CSS code to make our project beautiful. In terminal type `npm i bootstrap`. This will install the package into our project.

## Import Bootstrap

6. Then in VS Code, open the **/src/main.jsx** file and import the bootstrap css like by typing the following line `import 'bootstrap/dist/css/bootstrap.css';` placing it just after the import for ReactDOM and just before our import for **index.css**. This way we can override the bootstrap styles with our own inside index.css if we wish to.

## Exercise Assets

7. Move the image files from the `assets` directory outside the React project directory into the directory `public`. This way the images will be accessible to your application.

## Creating the App Component

8. Open **/src/App.jsx**. This file is an example component that React starts with. You can delete everything in this file. Then at the top of the file you can import React and create a functional component named `App`. Don't forget to export it.

9. Create a `<div>` inside of the `return()` statement.

10. Add `className="App container-fluid"` into the `<div>` element. This will apply some CSS styles to it.

```jsx
function App() {
  return <div className="App container-fluid"></div>;
}

export default App;
```

11. Then inside the `<div>` create a heading `<h1>My Travel Blog</h1>`.

```jsx
function App() {
  return (
    <div className="App container-fluid">
      <h1>My Travel Blog</h1>
    </div>
  );
}
```

12. Save the file and visit the browser to make sure our heading is appearing.

13. Back inside **/src/App.jsx** below our heading place `<div className="row"></div>`.

```jsx
function App() {
  return (
    <div className="App container-fluid">
      <h1>My Travel Blog</h1>
      <div className="row"></div>
    </div>
  );
}
```

Your task is to create an `articles` array of at least 3 article objects.
Each article has: id, title, body, and img.

Define the `articles` array in App.jsx.

Create
- an ArticleList component that uses map to render articles
- an Article component that renders a single article
