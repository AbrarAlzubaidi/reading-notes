# Next.js

## Assests
- Next.js can serve static assets, like images, under the top-level public directory.
- `next/image`: This allows for resizing, optimizing, and serving images in modern formats like WebP when the browser supports it. This avoids shipping large images to devices with a smaller viewport. It also allows Next.js to automatically adopt future image formats and serve them to browsers that support those formats.

Ex: 
```
import Image from 'next/image'

const YourComponent = () => (
  <Image
    src="/images/profile.jpg" // Route of the image file
    height={144} // Desired size with correct aspect ratio
    width={144} // Desired size with correct aspect ratio
    alt="Your Name"
  />
)
```

## Metadata
- modify metadata in head component
- `next/script`: is an extension of the HTML `<script>` element and optimizes when additional scripts are fetched and executed.
`import Script from 'next/script'`


## CSS Styling
- Next.js has built-in support for CSS and Sass which allows you to import .css and .scss files.
- `classnames`: is a simple library that lets you toggle class names easily. You can install it using `npm install classnames`


-----


# React context
## what is it?
React context allows us to share data (state) across our components more easily.

## When should you use React context?
passing data that can be used in any component in your application.

<p style='color:#F14A16;font-size:25px'>These types of data include:</p>

1. Theme data (like dark or light mode)
2. User data (the currently authenticated user)
3. Location-specific data (like user language or locale)

*Data should be placed on React context that does not need to be updated often.*

<spam style='color: #370665;font-size:15px'><b>Props drilling</b> </spam> is a term to describe when you pass props down multiple levels to a nested component, through components that don't need it.

<p style='color:#F14A16;font-size:25px'>four steps to using React context:</p>

1. Create context using the createContext method.
2. Take your created context and wrap the context provider around your component tree.
3. Put any value you like on your context provider using the value prop.
4. Read that value within any component by using the context consumer.

<p style='color:#FC9918; font-size:20px '>Resorces</p>

<button style='background-color:#FC9918;border-radius:5px'><a href='https://canvas.instructure.com/courses/3671304/discussion_topics/12904564' style='color:#370665'>read link</a></button>

<button style='background-color:#370665;border-radius:5px'><a href='https://nextjs.org/learn/basics/getting-started' style='color:#FC9918'>nextjs</a></button>

<button style='background-color:#370665;border-radius:5px'><a href='https://www.freecodecamp.org/news/react-context-for-beginners/' style='color:#FC9918'>react-context</a></button>
