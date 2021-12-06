# django forms

A HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server.

**html form**

    <form action="/team_name_url/" method="post">
        <label for="team_name">Enter name: </label>
        <input id="team_name" type="text" name="name_field" value="Default name for team.">
        <input type="submit" value="OK">
    </form>

The submit input will be displayed as a button (by default) that can be pressed by the user to upload the data in all the other input elements in the form to the server (in this case, just the team_name). The form attributes define the HTTP method used to send the data and the destination of the data on the server (action):

- action: The resource/URL where data is to be sent for processing when the form is submitted. 
- method: The HTTP method used to send the data: post or get.
   - The POST method should always be used if the data is going to result in a change to the server's database 
   - The GET method should only be used for forms that don't change user data 

## Django's form handling
Django's form handling uses all of the same techniques that we learned about in previous tutorials (for displaying information about our models): the view gets a request, performs any actions required including reading data from the models, then generates and returns an HTML page (from a template, into which we pass a context containing the data to be displayed). What makes things more complicated is that the server also needs to be able to process data provided by the user, and redisplay the page if there are any errors.

**form in django**

    from django import forms

    class RenewBookForm(forms.Form):
        renewal_date = forms.DateField(help_text="Enter a date between now and 4 weeks (default 3).")

**most fields in form**

- required: If True, the field may not be left blank or given a None value. Fields are required by default, so you would set required=False to allow blank values in the form.

- label: The label to use when rendering the field in HTML. If a label is not specified, Django will create one from the field name by capitalizing the first letter and replacing underscores with spaces (e.g. Renewal date).

- label_suffix: By default, a colon is displayed after the label (e.g. Renewal date:). This argument allows you to specify a different suffix containing other characters (s).

- initial: The initial value for the field when the form is displayed.

- widget: The display widget to use.

- help_text: Additional text that can be displayed in forms to explain how to use the field.

- error_messages: A list of error messages for the field. You can override these with your own messages if needed.

- validators: A list of functions that will be called on the field when it is validated.

- localize: Enables the localization of form data input.

- disabled: The field is displayed but its value cannot be edited if this is True. The default is False.