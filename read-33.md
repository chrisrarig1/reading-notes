# React 3

- *Next.js* is a React Framework

## Setup

### Create App

- `npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn/tree/master/basics/learn-starter"`

- Run dev server:
  - `npm run dev`
- Edit page:
  - `pages/index.js`

## Navigate through Pages

- Pages are associated with a route based on their file names
- `pages/index.js`: `/` route
- `pages/posts/first.js`: `/posts/first` route

## Creating a New Page

- Using above example create a file called first in a directory called posts
- Use the following setup in first:

```JS
export default function FirstPost() {
  return <h1>First Post</h1>
}
```

### Link Component

- `import Link from 'next/link`
- Update `<a>` tags to be surrounded by `<Link href=''>`

## Assets, Metadata, and CSS

- Next.js can serve static assets under the top level public directory
- images: `<img src="" alt=""/>`
- Size: `height={144}` `width={144}`
- *CSS*

```CSS
  .container {
  max-width: 36rem;
  padding: 0 1rem;
  margin: 3rem auto 6rem;
}
```

`import styles from './layout.module.css'`
`className={styles.container}`

## React Context for Beginners

- React context allows the passing down and use of data in any component without using props
- Use React context when sharing Theme data, User data or Location data

```JS
import React from 'react';

export const UserContext = React.createContext();

export default function App() {
  return (
    <UserContext.Provider value="Reed">
      <User />
    </UserContext.Provider>
  )
}

function User() {
  const value = React.useContext(UserContext);  
    
  return <h1>{value}</h1>;
}
```

# Useful Links

- [Next.js](https://nextjs.org/learn/foundations/about-nextjs?utm_source=next-site&utm_medium=homepage-cta&utm_campaign=next-website)
- [React Context for Beginners](https://www.freecodecamp.org/news/react-context-for-beginners/)
