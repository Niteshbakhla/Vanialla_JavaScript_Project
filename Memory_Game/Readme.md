In the browser: Your JavaScript works fine with import/export because modern browsers support ES Modules (<script type="module">).
In Node.js: You're getting errors because Node.js does not support ES Modules by default. It uses CommonJS modules (with require() and module.exports) by default.

Browser: Works fine with ES Modules.
Node.js: You must explicitly tell Node to use ES Modules by using .mjs or "type": "module" in package.json.