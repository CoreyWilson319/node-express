# node-express

# Step 1
Create the repo in github and clone that repo
# Step 2
In your terminal enter 
```
npm init
```
# Step 3
Answer the prompts as needed. Whatever is in parenthesis is the default.

# Step 4
Use module.exports to export functions. (Example below)
```js
module.exports = {
    add, 
    subtract,
    beBasic,
    addAgain
}
```

# Step 5
Use require to use those functions in a different js file. (Example below)

```js 
const {add, subtract,addAgain, beBasic } = require("./myModule");
```

# Step 6
To run the js file in the terminal enter node (filename.js)
```
node index.js
```

## To Install ndm packages

# Step 1
In the terminal enter npm i (name) or npm install g (name) to install globally

```
npm i ascii-art
```

# Step 2
In your Javascript file add the package using require(name) use the bottom to include local modules you have made the quotation marks have the file directory

```
const {fullName} = require("./myModule");
const style = require('ansi-styles');
```

# Step 3
Follow package documentation to learn how to use the package you've included now into your js file.

## To use express
# Step 1

require express and use ejs if wanted
```js
const express = require('express');
const app = express();

app.set('view engine', 'ejs')
```

# Step 2
use .get to create the route so for example use
```js
app.get('/', function(req, res){
    // res.sendFile(__dirname + '/views/index.html');
    // res.status(200)
    res.render('index', { myVar: "woohoo"})
});
```

__dirname grabs the directory of the root repo

# Step 3 to send html
Use res.sendFile  to send a file to the route such as an html file
```js
   // res.sendFile(__dirname + '/views/index.html')
   ```
   
# Step 3 to send text use

```js
res.send()
```

# Step 4 to reference variables use icecream cone notation
```html
<%= myVar %>
```
