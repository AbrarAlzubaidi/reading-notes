## forms: 
to collect information from users.

#### forms type:
1. adding texts:
    1. text input: to add single line.
    2. password: to add password.
    3. text area: to add multi-line.

2. making choice:
   1. radio buttons: select one of the options.
   2. checkbox: select one or more options.
   3. drop down box: make a list.

3. submitting forms:
    1. submit button: to submit data.
    2. image button: to add img.
    3. upload: to upload files.


#### how to add forms in html:
using `<form>` tag holds the attributes:

   1. action: URL for the page on the server.
   2. method:holds 2 values:
        1. get: values will add to the end of URL.
        2. post: values send with http headers.

#### to add text input:
inside the form tage `<input>` attributes:

1. type: value:text to add single line.
2. name: its name.
3. size: its size.
4. maxlength: to limite number of characters.


#### to add pass input:
inside the form tage `<input>` attributes:

1. type: value:password to add password
2. name: its name.
3. size: its size.


#### to add text area input:
inside the form tage `<textarea>` attributes:

1. name: its name.
3. rows: number of rows.
4. column: number of column.

#### to add radio button:
inside the form tage `<input>` attributes:

1. type: value:radio.
2. name: its name.
3. value: its value.
4. checked: which values should be selected when the page loads.

#### to add checkbox:
inside the form tage `<input>` attributes:

1. type: value:checkbox
2. name: its name.
3. value: its value.
4. checked: which values should be selected when the page loads.

#### to add dropdown box:
inside the form tage `<select>` attributes:

1. name: its name.
2. size: number of options that you want to show it at once.
3. multiple: to select multiple options.

#### to add file input:
inside the form tage `<input>` attributes:

1. type: value:file
2. name: its name.
3. type: value: submit: to upload the value


#### to add img button:
inside the form tage `<input>` attributes:

1. type: value:image
2. src: img link


#### to add buttons:
inside the form tage `<button>` 


------------------------------------------


### labels:
each form have its own label.`<label>`


#### grouping forms:

1. `<fieldset>` to create group form.
2. `<legend>`: name to identify the purpose of this grouping.
3. value: its value.
4. checked: which values should be selected when the page loads.


#### to add date input:
inside the form tage `<input>` type attribute value = date.

#### to add emails and URL:
inside the form tage `<input>` type attribute value = email/url.

#### to add search input:
inside the form tage `<input>` type attribute value = search.


---------------------------------------


### lists: 
order and un-orderd list

attributes:

1. `list-style-type`: to style the list.
2. `list-style-img`: to replace the decimal numbers into imgs.
3. `list-style-position`: inside or outside.

#### table properties:
you can style the table using some attributes such as:

1. width.
2. border.
3. letter-spacing
4. text-transform


#### you can show borders in an empty cell or not py:
empty-cell property:

1. show: to show it
2.  hide: to hide it
3. inherit.

#### to add gaps between cells:
1. border-spacing.
2. border-collapse
   1. collapse: make it to a single border for all cells.
   2. separate: each cell has its border and thry are separated.


--------------------------------------------


## events:
simple, events are actions that happen in the system. if something happens.like click on the buttons.

to add event:

        <element eventname='some JavaScript'>


Events can be used to verify user input, user actions, and browser actions, like:

1. Things that should be done every time a page loads, like update the date and the time when the user open the page
2. Things that should be done when the page is closed, like pop a msg tell him to rate the page.
3. Action that should be performed when a user clicks a button
Content that should be verified when a user inputs data, like to calculate some data.
