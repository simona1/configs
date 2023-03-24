# Express

## Installation

```
yarn add --exact express
```

## Usage

Below is a Hello World example, that was slightly modified from the [official example](https://expressjs.com/en/starter/hello-world.html):

```js
const express = require("express");

const PORT = 3000;

const app = express();

app.get("/", (req, res) => {
  res.send("Hello World!");
});

app.listen(PORT, () => {
  console.log(`Example app listening on port ${PORT}`);
});
```

To start the server by running it with `node`, do:

```
node src/server/main.js
```

To run it with `yarn`, add a script to your `package.json`:

```json
{
  "scripts": {
    "start": "node src/server/main.js"
  }
}
```

## Additional

For an Express with Typescript project, install these dev dependencies:

```
yarn add --dev --exact @types/express @types/node
```
