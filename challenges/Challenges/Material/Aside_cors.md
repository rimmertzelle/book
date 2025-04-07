# Aside  - Cors

When working with AJAX and JavaScript, it's common to encounter Cross-Origin Resource Sharing (CORS) errors. CORS is a security measure that prevents JavaScript from making requests across domain boundaries. Here are a few methods to handle this issue:

1. **Use CORS Headers**: If you have control over the server, add appropriate CORS headers there. Here's an example of how you might set it up in an Express.js server:

```jsx
app.use(function(req, res, next) {
  res.header("Access-Control-Allow-Origin", "*");
  res.header("Access-Control-Allow-Headers", "Origin, X-Requested-With, Content-Type, Accept");
  next();
});

```

1. **Use a Proxy**: If you don't have control over the server, you may need to use a proxy. You can set up your own proxy server, or use an existing one.

Please note, these methods should be used as per your project's security guidelines and requirements.

If you need the use a proxy, we have you covered. Read the following article and use the provided `php` setup.

[API proxy](Aside%20-%20Cors%2071b5eadfe9204810a4f6a915fc3019e5/API%20proxy%20ff1eb2642a1a4300b2b6482bae6a29a9.md)

### Further reading

---

[✋🏼🔥 CS Visualized: CORS](https://dev.to/lydiahallie/cs-visualized-cors-5b8h)