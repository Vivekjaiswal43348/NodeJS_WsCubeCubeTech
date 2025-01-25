

# Project Code-1
Project Credit : [WsCube Tech YTube](https://www.youtube.com/watch?v=vfaRzV3P92o)

## Basic Project Config
1. npm init -y
2. node index.js
3. npm i -g nodemon
    run in Powershell terminal to enamble nodemon command:
    "Set-ExecutionPolicy RemoteSigned -Scope CurrentUser"
4. Configure start command in Package script: `"start": "nodemon index"`

 ```   
"scripts": {
    "start": "nodemon index",
    "test": "echo \"Error: no test specified\" && exit 1"
}
```

## Types of Modules
- `core modules` : Already available with node JS (FS, HTTP, PATH)
- `custom modules`: build by developer
- `Third-party modules`: we can import from 3rd party libraries(Express JS, Next JS, NPM)

## type commonjs vs type module in package.json file
- in commonjs we use require for import of class, function, variable etc.
    by default type is commonjs
    `"type": "commonjs",`
- in module we use import statement just like in ReactJS
    `"type": "module",`

## Topic wise learning
 1. Create a module and export it
 2. Type of export: default export and named export
   ##### Default export and import:
```
     Export
        const addToCart = () => {
            return "Add to cart";
        };

        module.exports = addToCart;
   
     Import
        const addToCart = require("./cartModule");
```
   ##### Named export and import:

```
     Export
       const addToCart = () => {
            return "Add to cart";
        };

        const changeQty = () =>{
            return 5;
        }
        module.exports = {addToCart,changeQty};
   
     Import
        const {addToCart,changeQty} = require("./cartModule");
```


## Creating a server in NodeJS(seperate repo/local project)