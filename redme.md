
Project Credit from [WsCube Tech YTube](https://www.youtube.com/watch?v=vfaRzV3P92o)

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
- core modules : Already available with node JS (FS, HTTP, PATH)
- custom modules: build by developer
- Third-party modules: we can import from 3rd party libraries(Express JS, Next JS, NPM)

## commonjs vs modules
- in common js we use require for import of class, function, variable etc.
- in module we use import statement just like in ReactJS