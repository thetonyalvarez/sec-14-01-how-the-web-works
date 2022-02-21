## Part One: Solidify Terminology

In your own terms, define the following terms:

What is HTTP?

> Hyper Text Transfer Protocol

What is a URL?

> The address of a webpage. Made of the following parts:
> Ex: `http://example.com/some/page.html?results=3`
>
> -   Protocol => `HTTP` or `HTTPS`
> -   Hostname => `example.com`
> -   Port => `80` for `HTTP`, `443` for `HTTPS`
> -   Resource => `/some/page.html`
> -   Query => `?results=3`

What is DNS?

> Domain Name Server. Translates a hostname into a numeric IP address.

What is a query string?

> Arguments appended at the end of a URL that provide extra info in the request - search terms, form info, etc.

What are two HTTP verbs and how are they different?

> `GET`
>
> -   Requests **without** side effects (don't change server data)
> -   Arguments are usually passed along in query string
> -   If you know arguments, you can change the URL
> -   Can be sent by entering-URL-in-browser, clicking links, and **some** form submissions
>
> `POST`
>
> -   Requests **with** side effects (**change data** on server)
> -   Arguments are sent in body of the request body, not in query string
> -   **Some** form submissions, but NEVER via entering-URL-in-browser, or links
> -   **Always** do this if there's a side effect: sending email, charging credit cards, etc.

What is an HTTP request?

> HTTP protocol that uses the `GET` method to request information from a server.
>
> -   Sends info inside `header`
>     -   Hostname you're asking about
>     -   Date your browser thinks it is
>     -   Language your browser wants it in
>     -   Cookies that server sent

What is an HTTP response?

> HTTP protocol that uses the `POST` method to retrieve information from a server.
>
> -   Sends a Response Status Code (200, 404, etc)
> -   `Header` includes:
>     -   Content Types (typically `text/html` for web pages)
>     -   Date/time the server thinks it is
>     -   Any cookies the server wants to set
>     -   Any caching info

What is an HTTP header? Give a couple examples of request and response headers you have seen.

> Information in an HTTP verb that details the info that your verb is looking for:
>
> `GET` example:
>
> ```
> GET /demo.css HTTP/1.1
> Host: site.com
> Date: [date browser thinks it is]
> Cookie: [any cookies browser is storing for that host]
> ...
> ```
>
> `POST` example:
>
> ```
> HTTP/1.1 200 OK
> Date: [date server thinks it is]
> Content-Type: text/css
> Cookie: [any cookies server wants you to set]
> ...
>
> body {
>   background-color: lightblue;
> }
> ...
> ```

What are the processes that happen when you type [http://somesite.com/some/page.html](http://somesite.com/some/page.html) into a browser?

> -   Turn `somesite.com` into IP address (ex. `123.45.67.89`)
> -   Connect to `123.45.67.89`
> -   On port 80 by default
> -   Using HTTP protocol
> -   Ask for `some/page.html`
