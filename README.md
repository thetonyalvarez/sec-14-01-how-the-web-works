# How Web Works Exercise

## Part One: Solidify Terminology

[Click here to view answers to Part 1.](part-1.md)

---

## Part Two: Practice Tools

1. Using `curl`, make a `GET` request to the _icanhazdadjoke.com_ API to find all jokes involving the word “pirate”
1. Use `dig` to find what the IP address is for _icanhazdadjoke.com_
1. Make a simple web page and serve it using `python3 -m http.server`. Visit the page in a browser.

---

## Part Three: Explore Dev Tools

Build a very simple HTML form that uses the `GET` method (it can use the same page URL for the action) when the form is submitted.

Add a field or two to the form and, after submitting it, explore in Chrome Developer tools how you can view the request and response headers.

Edit the page to change the form type to `POST`, refresh in the browser and re-submit. Do you still see the field in the query string? Explore in Chrome how you can view the request and response headers, as well as the form data.

---

## Part Four: Explore the URL API

At times, it’s useful for your JavaScript to look at the URL of the browser window and change how the script works depending on parts of that (particularly the query string).

[Read about the URL API](https://developer.mozilla.org/en-US/docs/Web/API/URL)

Try some of the code examples in the Chrome Console so that you can get comfortable with the basic methods and properties for instances of the URL class.
