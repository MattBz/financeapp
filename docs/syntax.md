# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5

* `bold and boxed list item`
* **bold list item**
* [Google.de](http://google.de)
* list item

>**Note**

> Note text


```
my-app/
  public/
    index.html
    favicon.ico
  src/
    App.css
    App.js
```

```
/             - static server returns index.html with React app
/todos        - static server returns index.html with React app
/api/todos    - server handles any /api/* requests using the backend implementation
```

```json
{
  "version": "0.2.0",
  "configurations": [{
    "name": "Chrome",
    "type": "chrome",
    "request": "launch",
    "url": "http://localhost:3000",
    "webRoot": "${workspaceRoot}/src",
    "userDataDir": "${workspaceRoot}/.vscode/chrome",
    "sourceMapPathOverrides": {
      "webpack:///src/*": "${webRoot}/*"
    }
  }]
}
```

```js
import React, { Component } from 'react';

class Button extends Component {
  render() {
    // ...
  }
}

export default Button; // Don’t forget to use export default!
```

```css
.App {
  display: flex;
  flex-direction: row;
  align-items: center;
}
```

```html
<div>
  <small>You are running this application in <b>development</b> mode.</small>
  <form>
    <input type="hidden" value="abcdef" />
  </form>
</div>
```

```bash
npm install project
npm start
```
