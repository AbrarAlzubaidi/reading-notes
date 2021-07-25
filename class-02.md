## Text in html:
by determine the importance of your text you can use heading tags.
from `<h1>` to `<h6>`.`<h1>` contains the most important heading, `<h6>` contains the least important heading.

- if the text is a paragraph you can use `<p>` tag
- `<b>` for bold text.
-  `<i>` italic text.
- `<sup>` to contain characters that superscript.
- `<sub>` to contain characters that subscript.
- `<br />` it is a self closing tag to make new line.
- `<hr />` also is a self closing tag to create a break (line) between elements like between 2 paragraphs.
- `<strong>` to make some text more strong importance. browser will understand it.
- `<em>` to define emphasized text.
- `<blockquote>` for long quotes.
- `<q>` for short quotes.
- `<abbr>` to define shortcuts like html, who (refers to person).
- `<cite>` to referance something like the auther name.
- `<del>` make a line on the text to mean this text deleted.
----------------------------------------------------

## CSS 
cascade style sheet, it allows you to create rules that control each elements representing (format/style your page).

**Css** can applied in 3 ways:

1. inline: inside an opening tag
    `<h1 style="attribute:value>   Something <h1>   "`
    this way will applied for the element that defines it.
2. internal: inside `<style>` tag.

**Rules contains two parts:**

1. selectors: means which element the rules will be appllied to it. there are many type of selectors such as: universal (`* {}`) all elements will be applied the same rules, type (`h1{}`) by type element's name all rules inside this selector will applied to the same element's name, class (`. {}`) to make some rules applied for seversl elements, id (`# {}`) to make some rules applied for specific element...etc.
2. declaration: how the element reffered to in the selector should be styled. 

- to link Css code in html file using `<link> tag `
- you can use Css internally in html using `<style>` tag but it is not the best practice.

