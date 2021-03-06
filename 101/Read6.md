# CSS:

CSS (Cascading Style Sheets) allows you to create great-looking web pages.

- Presenting a document to a user means converting it into a form usable by your audience. 
- h1 {
    color: red;
    font-size: 5em;
}

### CSS Modules:
- As there are so many things that you could style using CSS, the language is broken down into modules.

### CSS Specifications:
- CSS is defined in giant documents called specifications, which are published by standards organizations.
- CSS is constantly developing, with new features coming available.


### style rule syntax:

 style-rule ::=

    selectors-list {
      properties-list
    }

... where :

selectors-list ::=

    selector[:pseudo-class] [::pseudo-element]
    [, selectors-list]

properties-list ::=

    [property : value] [; properties-list]




**like:**

1. p{
   ... element selector:selects HTML elements based on the element name
}

2. *o{
  ....  universal selector:selects all HTML elements on the page
}

3. #d{
  ....id selector: to select a specific element(one element)
}

4.   .c{
  ... class selector:select a specific class attribute(more than one element)
}

5. h1{
   ... grouping selector:selects all the HTML elements with the same style definitions.
}


- selectors: allow styles to be conditional based on various features of elements within the DOM

- Basic selectors are fundamental selectors; these are the most basic selectors that are frequently combined to create other, more complex selectors.


# CSS Tools: Reset CSS:

The goal of a reset stylesheet is to reduce browser inconsistencies in things like default line heights, margins and font sizes of headings, and so on.

- The reset styles given here are intentionally very generic. There isn't any default color or background set for the body element

