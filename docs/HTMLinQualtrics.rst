.. _HTML:

=============================================
HTML in Qualtrics
=============================================
Qualtrics allows you to use customized HTML and CSS to design and format your survey questions.
This section explains how to use customized HTML, the difference between Rich Content Editor and HTML View, and the connection to JavaScript.

HTML and CSS in Qualtrics
=========================
To add custom HTML and CSS in Qualtrics, you can use the Rich Content Editor or directly edit the HTML.

Rich Content Editor
___________________________
The Rich Content Editor in Qualtrics allows you to format text, add images, and create tables using a graphical interface without writing any HTML code.
For our template, it is quite useful as it also allows you to edit RAW HTML and CSS within the editor, and the visual result is immediately displayed in the editor.

.. image:: pythonProject/docs/_static/HTMLPicture1.png
  :width: 400

By clicking on the 'Source' button, which is located in the top row of the editor, you can edit the HTML and CSS code directly.

.. image:: pythonProject/docs/_static/HTMLPicture2.png
  :width: 400

CSS in Qualtrics
========================
With CSS, you can style the individual HTML elements in your survey.
It is important that the CSS code is placed within a style block.

.. code-block:: console

    <style type="text/css"> Costum CSS </style>

Here, the page can be defined in the usual CSS manner.
It is important to define style classes.
You choose a name, for example, ExampleClass, prepend a period to the name, and place curly brackets after the word, within which the CSS code can be placed.

.. code-block:: console

    .ExampleClass {
         ...
        }

To apply this style to individual HTML elements, simply assign the class to those elements.

Example

.. code-block:: console

    <div class="ExampleClass"> Text </div>
    <label class="ExampleClass" type="radio"> Option 1 </label>
    <button class="ExampleClass"> Button Text </button>
    ...
