# Props + Iteration Exercise: Travel Blog

## Setup

Create a new React app with Vite.

---

## Assignment

Build a simple travel blog page that displays a list of articles.

Your app should be broken into **multiple components** and use **props** to pass data between them.

---

## Requirements

### Data 

Create an `articles` array with at least 3 objects.

Each article must have:
- `id`
- `title`
- `body`
- `img` (path to an image in your `public` folder)
- `featured` (true/false)

---

### Components

You must have:
- `ArticleList`
- `Article`

---

### Goal

Display all articles on the page.

Each article should show:
- Title  
- Body  
- Image  

If an article is featured, display something like:
**"Featured Post"**

---

## Notes

- Images should live in the `public` folder (ex: `/images/bonaire.jpg`)

---

## Basic Styling

Add this to your `index.css`:

```css
body {
  font-family: Arial, sans-serif;
  margin: 0;
  background-color: #f5f5f5;
}

.App {
  max-width: 900px;
  margin: 0 auto;
  padding: 20px;
}

h1 {
  text-align: center;
}

.article-list {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.article {
  background: white;
  padding: 16px;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}

.article img {
  width: 100%;
  border-radius: 6px;
  margin-bottom: 10px;
}

.article h2 {
  margin: 0 0 10px;
}
