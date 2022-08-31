## 01 Module

### Simple introduction:

 Why type js?
 > `To avoid possible bugs in development, the use of typing helps when debugging the code.`

How it works?
 > `The browser cannot interpret the code in ts.`
 > `You need to port it to an ECMAScript version.`


### How to install TS:

You need node.js and npm package management (yarn)

To install TS:

```bash
  npm instal typescript
```

It is possible to install globally, to do so use the -g flag:
```bash
  npm instal -g typescript
```
###  Run Manually

* create the file.ts file with the following code:
```
  const a: string = "First TS code"
  console.log("a: ", a)
```

* Now open the terminal and go to the project directory that the file is in and run it: 

```bash
  tsc file.ts
```

* Notice that a new file has been created in the root of the folder with the same name, but with the file extension being js.
* And now you can run firts.js in the terminal and see the message: `First TS code`.


### Set up the TS compiler

* You can configure it:
    - Define the location of the `.ts` files within the project.
    - The directory of destination transposed files.
    - The version of ECMAScript.
    - The restriction level of the type checker.
    - If the compiler should allow `.js` files.

To setup the compiler you need to generate the `tsconfig.json` file, run it in the project terminal:

```
    tsc --init
```

This command created a file in the project root with default settings (each rule comes with an explanatory comment).

#### To improve the experience when developing with TS we can automate the compilation process.

* Just pass the `w` parameter in front of the `tsc` command:
```
    tsc -w --p tsconfig.json
```