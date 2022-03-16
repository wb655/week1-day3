# VetsInTech Introduction to Web Development

## Week 1 Day 3

### Comments

"In computer programming, a comment is a programmer-readable explanation or annotation in the source code of a computer program. They are added with the purpose of making the source code easier for humans to understand, and are generally ignored by compilers and interpreters." (Wikipedia)

_The link to the resource is in the README_

We will revisit comments for each language we touch on: HTML, CSS, JS.

There are two styles of comment. The block (multi-line) comment and the line comment.

For HTML, the comment style is the same.

<!--- COMMENTS GO IN BETWEEN --->

As long as the arrow brackets are open, the contents will be comments, even across multiple lines.

<!---
This is a
multi-line
comment in HTML.
--->

### Tables

HTML tables allow web developers to arrange table cells of data into rows and columns.

#### Table Cells

Each table cell is defined by a <td> and a </td> tag.

td stands for table data.

Everything between <td> and </td> are the content of the table cell.

Note: table data elements are the data containers of the table.

They can contain all sorts of HTML elements; text, images, lists, other tables, etc.

#### Table Rows

Each table row starts with a <tr> and end with a </tr> tag.

tr stands for table row.

You can have as many rows as you like in a table, just make sure that the number of cells are the same in each row for an even table! You can have less cells per row.

#### Table Headers

Sometimes you want your cells to be headers, in those cases use the <th> tag instead of the <td> tag.

#### Table groups

- <thead>
- <tbody>
- <tfoot>
- <colgroup>
- <col>

#### I GO, YOU GO

Watch me first!

On your turn...

- Create a table, with a table header
- Header cells wll be First Name, Last Name, Occupation, Favorite Band
- Create 4 people and fill in all the data
- Create a fifth person that does not have a favorite band
- Create a sixth person who does not have an occupation

Make sure to view the content in your browser and make sure the content lines up!

### Forms

An HTML form is used to collect user input. The user input is most often sent to a server for processing.

#### The <form> Element

The HTML <form> element is used to create an HTML form for user input. It represents a document section containing interactive controls for submitting information.

There are optional attributes for the form with default behaviors.

- action: string/URL
- method: PUT, GET, DELETE, POST

The <form> element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.

#### Input Element

The HTML <input> element is the most used form element.

An <input> element can be displayed in many ways, depending on the type attribute.

- text
- radio
- checkbox
- submit
- button

The <input type="text"> defines a single-line input field for text input.

The form itself is not visible. Also note that the default width of an input field is 20 characters.

#### The <label> Element

The <label> tag defines a label for many form elements.

The <label> element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focus on the input element.

The <label> element also help users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the <label> element, it toggles the radio button/checkbox.

The for attribute of the <label> tag should be equal to the id attribute of the <input> element to bind them together.

<form>
  <label for="fname">First name:</label><br>
  <input type="text" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" name="lname">
</form>

#### The Submit Button

The <input type="submit"> defines a button for submitting the form data to a form-handler.

The form-handler is typically a file on the server with a script for processing input data.

The form-handler is specified in the form's action attribute.

## Exercise

Please create a new HTML page with:

- a h1 element with your name
- a h2 element with your occupation
- a ul list containing the skills you have/will obtain
- a h3 element with the text content "Let's get in touch!"
- a form with no action or method wrapped around:
  - a 2x3 table with no thead or th
    - each row will have the label and text input
      - full name
      - email
      - note
