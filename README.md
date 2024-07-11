# Rupert

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/agilecollective/rupert)

## Exercise: HTML form submission

- Create a HTML form which allows the input of a first and last name
- On submission of the form, send the data to the PHP script
- Get the PHP script to display `Hello [first name] [last name]`
- If either the first or last name is null/empty, display an error message.

### Resources
- https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form
- https://www.php.net/manual/en/reserved.variables.post.php
- https://www.php.net/manual/en/function.echo.php

### Questions
- What is the response status code?
- What is the request content type?
- Which HTTP method did the request use?
- What is PHP doing for us in this very simple application?
- What type of "rendering" is at play here?
- What alternative implementation could provide the same functionality?

## Exercise: handle form submission with JS

- Create a script file and link it to your HTML page.
- Set up an event listener for the form submission, grab the form values and post them as JSON to your PHP script.
- In the PHP script, concatenate your variables and respond with JSON.
- Receive the response on the frontend and display back to the user.

### Resources
- https://developer.mozilla.org/en-US/docs/Web/API/HTMLFormElement/submit_event
- https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch
- https://stackoverflow.com/questions/4064444/returning-json-from-a-php-script

## Exercise: use the Symfony HttpFoundation for the request and response

- Create a Composer file
- Use Composer to install the library (hint: Composer can be used in Lando by running `lando composer` in the terminal)
- Include the Composer autoloader in your PHP script
- Refactor your existing code to use the Symfony Request and Response objects instead of working directly with PHP globals.

### Resources

- https://symfony.com/doc/current/components/http_foundation.html#installation
- https://getcomposer.org/doc/01-basic-usage.md#autoloading
- https://symfony.com/doc/current/components/http_foundation.html#request
- https://symfony.com/doc/current/components/http_foundation.html#response
