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