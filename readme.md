# TypeScript_WebAppAutomation

# Instructions to Setup Cucumber typescript Project with Selenium

## Initialize your project
First, create a project directory and navigate into your new project root directory.

Next, intialize the project:

```agsl
npm init -y
```

Next, Set typescript as a dev dependency:

```agsl
npm install --save-dev typescript
```

Now we need to initialize our project with typescript:

```agsl
tsc --init
```

Now we have a couple dependencies we need to install for dev:

```agsl
npm install --save-dev @cucumber/cucumber
npm install --save-dev allure-cucumberjs
npm install --save-dev @types/node
npm install --save-dev selenium-webdriver
npm install --save-dev @types/selenium-webdriver
```

Now a dummy file used for convention(you can also just create one without command line):

```agsl
touch .dummy.txt
```

## Configure typescript

Let's configure typescript now! To do so, create the file tsconfig.json in your root directory:

```agsl
{
  "compilerOptions": {
    "module": "commonjs",
    "outDir": "./dist",
    "target": "ES2022",
    "lib": ["ES2022"],
    "esModuleInterop": true,
    "skipLibCheck": true
  },
  "include": [
    "./features/step_definitions/**/*",
    "./features/support/**/*"
  ]
}
```




