# API proxy

All code on: [https://github.com/rimmertzelle/ajax-proxy](https://github.com/rimmertzelle/ajax-proxy)

### What is a proxy?

In this case a proxy is a middle man on the server which handles the request and the response to an API. The API is not directly contacted via JavaScript (AJAX) on the client/browser. There are two reasons to setup a proxy. 

**Security**

When you run code in the browser that contains a request to code from a different domain, for example via an API call, you violate some security rules and this error might popup.

![[https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fproxyman.io%2Fblog%2Fassets%2Fimages%2Fhow-to-by-pass-cors-policy%2Fhow-to-by-pass-cors-policy-3.png&f=1&nofb=1](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fproxyman.io%2Fblog%2Fassets%2Fimages%2Fhow-to-by-pass-cors-policy%2Fhow-to-by-pass-cors-policy-3.png&f=1&nofb=1)](API%20proxy%20ff1eb2642a1a4300b2b6482bae6a29a9/Untitled.png)

[https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fproxyman.io%2Fblog%2Fassets%2Fimages%2Fhow-to-by-pass-cors-policy%2Fhow-to-by-pass-cors-policy-3.png&f=1&nofb=1](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fproxyman.io%2Fblog%2Fassets%2Fimages%2Fhow-to-by-pass-cors-policy%2Fhow-to-by-pass-cors-policy-3.png&f=1&nofb=1)

It says No 'Access-Control-Allow-Origin' header is present on the server (resource). So the API/server has not implemented cross domain requests correctly (or the request is directly called from your filesystem, instead of a server).

**Authentication**

Most of the times you have to authenticate your request to an API. You can add your credentials to the JavaScript file, however, this is not a really smart thing to do. Every person with a browser has access to your credentials. Via a proxy you can hide your credentials.

### Some code examples

---

[Working example](API%20proxy%20ff1eb2642a1a4300b2b6482bae6a29a9/Working%20example%20b6a071b725b748fd8695484ce2b142ac.md)