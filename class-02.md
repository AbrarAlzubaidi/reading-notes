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
3. external: it is the best way because it will reduce errors and conflicts that will happen in previous ways amd make maintaine process much easier.

**like html Css has versions** Css1,Css2,Css3

**Rules contains two parts:**

1. selectors: means which element the rules will be appllied to it. there are many type of selectors such as: universal (`* {}`) all elements will be applied the same rules, type (`h1{}`) by type element's name all rules inside this selector will applied to the same element's name, class (`. {}`) to make some rules applied for seversl elements, id (`# {}`) to make some rules applied for specific element...etc.
2. declaration: how the element reffered to in the selector should be styled. 

- to link Css code in html file using `<link> tag `
- you can use Css internally in html using `<style>` tag but it is not the best practice.

------------------------------------------------------------------

## JS

in JS each line of code called statement. JS is a case sensitive language, you should be carefull about this point, which means (name different from Name different from NAME ...etc).

### how to apply commints in JS:
//----> this for single line commint like 

          //  single commint


/*    */ ----> this for multi-line commint.like

         /* multi
             line
               commint   */

### variables: 
it is like a space that stores data.its value could change or still as it.

**How to declare it**
you can use `var OR let` keywords

ex: 

     var variavleName;
     var x;
     let y;


**How to assign it**

by using assignement operator.
ex:

    var x=6;
 

**variable datatypes**

1. number: it can be any number int, float,...etc
2. boolean: true or false
3. string: anything inside double-quotation or single-quotation.


**rules to name variables:**

1. must begin **just**with letter,$,_
2. not a keyword.
3. can contain numbers,symbols except (. and -)
4. they are case sensitive
5. make sure name it depends on its purpose to make it easy to understand what is this variable


## Arrays
it's a special type from variables can store more than one value.

**How to declare it and assign it**

ex:
     
      var num=[1,2,3,4,5];
      let type=["int","string","bool"];


arrays have something special called **index**

index it is a number refers to array's element position. start from 0 which referes to first element to (no.of elements-1) which refers to last element.

in previous example num array has 5 elements 
if i want to applied this it will be:


|element|index|
|-------|-----|
|1      |0    |
|2      |1    |
|3      |2    |
|4      |3    |
|5      |4    |


to know array's length (how much elements it have?) ---> called function 

       // arrayName.length();
       num.length();   // will print 5

  
to print specific element---->

     // arrayName[index];
     num[2];   // will print 3



## operators type:
1. arithmatic: +,-,*,/,%,++,--
2. assignement =
3. logical  && (and),|| (or) ,!(not)


**and logic table**


|input        |output|
|-------------|------|
|0 and 0      |0     |
|0 and 1      |0     |
|1 and 0      |0     |
|1 and 1      |1     |


**or logic table**

|input        |output|
|-------------|------|
|0 or 0       |0     |
|0 or 1       |1     |
|1 or 0       |1     |
|1 or 1       |1     |


** not logic table**


|input     |output|
|----------|------|
|not 0     |1     |
|not 1     |0     |




4. comparision ==,!=,!==,===,<,>


## conditional statement:
use it if you want to copmaire somthing, if there is a condition have true and false probabilities.

syntax
 
      if(condition)
      {
        // if condition true do this block of code
      }
      else {
        // if condition false do this block of code
      }