# Sending and Retrieving Form Data
 This summary explains what happens when a user submits a form (e.g. where the data goes, how do we handle it when it gets there?, etc), as well as a security concern associated with sending form data.

## Client/server architecture
At it's most basic, the web uses a client/server architecture that can be summarized simply: a client (such as a web browser) sends a request to a server (such as Node.js), using HTTP protocols and the server resonding in same. We will now look at both sides to the equation, starting with the client side.

## HTTP Methods
The <form> element determinse how to send the data. Its attributes are designed to onfigure the request to be sent when a user hits a submit button - no need to write extra code. The two most important attributes, however, are action and method. Method, as the name implies, determines the method of sending the data, (Namely, GET or POST).

POST is important for two reasons:

1. If you need to send secure data, such as a password. Using GET method would mean displaying the content in the URL bar, which would be bad.
1. If you need to send a large amount of data.  Browsers limit the sizes of URLs, and further, many servers limit the length of URLs they accept. Thus, long amounts of data need to be stored somewhere else besdies within the URL.

Whichever HTTP method you choose, the server receives a string that will be parsed and then dealth with. 

## A special case: sending files
Not all kinds of data were originally meant to be sent via HTTP. For example, files are binary data, (or treated that way), but all other data is, or is considered, text data. HTTP is a text protocol, thus it was never meant to deal with binary data. We need to make some special adjustments.

Enctype defines the MIME type of the information sent to the server (assuming the method used is POST). There are three options:

1. enctype="application/x-www-form-urlencoded"
1. enctype="text/plain"
1. enctype="multipart/form-data"

By default, its value is application/x-www-form-urlencoded. In human terms, this means: "This is form data that has been encoded into URL parameters."

If you want to send files, you need to take three extra steps:

1. Set the method attribute to POST because file content can't be put inside URL parameters.
1. Set the value of enctype to multipart/form-data because the data will be split into multiple parts, one for each file plus one for the text data included in the form body (if text is also entered into the form).
1. Include one or more <input type="file"> controls to allow your users to select the file(s) that will be uploaded.


For more information, see: 

https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data

https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/forms

https://htmlreference.io/forms/

