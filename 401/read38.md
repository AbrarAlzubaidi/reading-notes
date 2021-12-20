# REACT.js

## Conditional Rendering
- You can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.

## Lists and Keys
1. Lists :
- use the map() function to iterate on array 

Ex:
```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
<li>{number}</li>
);

```
- Rendering Multiple Components
- You can build collections of elements and include them in JSX using curly braces {}.

2. Keys

- Keys help React identify which items have changed, are added, or are removed.

## Extracting Components with Keys
- Keys only make sense in the context of the surrounding array.

- For example, if you extract a ListItem component, you should keep the key on the <ListItem /> elements in the array rather than on the <li> element in the ListItem itself.


-------

# Forms

- form elements naturally keep some internal state.

- React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.

------


# Lifting State Up
- In React, sharing state is accomplished by moving it up to the closest common ancestor of the components that need it. This is called “lifting state up”.


------


# Thinking in React

- React is, the premier way to build big, fast Web apps with JavaScript. It has scaled very well for us at Facebook and Instagram.

- One of the many great parts of React is how it makes you think about apps as you build them.