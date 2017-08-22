# tdd-configuration
Configuration of TDD environment.

1. Create tdd folder: 
```bash
  mkdir tdd
```

2. Go to tdd folder: 
```bash
  cd tdd
```

3. Create Node tdd project: 
```bash
  npm init
```
**Result**:
```bash
{
    "name": "tdd",
    "version": "1.0.0",
    "description": "TDD Workshop",
    "main": "index.js",
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "author": "",
    "license": "ISC"
}
```

3. Install **Karma and Dependencies** from: 
```bash
  npm install -g karma-cli
  npm install karma --save-dev
  npm install karma-jasmine karma-chrome-launcher jasmine-core --save-dev
```

**Result**:
```bash
{
    "name": "tdd",
    "version": "1.0.0",
    "description": "TDD Workshop",
    "main": "index.js",
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "author": "",
    "license": "ISC",
    "devDependencies": {
        "jasmine-core": "^2.7.0",
        "karma": "^1.7.0",
        "karma-chrome-launcher": "^2.2.0",
        "karma-jasmine": "^1.1.0"
    }
}
```

4. Create a karma project with:
```bash
  karma init
```

**With the next configuration**:
```bash
Which testing framework do you want to use ?
Press tab to list possible options. Enter to move to the next question.
> jasmine

Do you want to use Require.js ?
This will add Require.js plugin.
Press tab to list possible options. Enter to move to the next question.
> no

Do you want to capture any browsers automatically ?
Press tab to list possible options. Enter empty string to move to the next question.
> Chrome
>

What is the location of your source and test files ?
You can use glob patterns, eg. "js/*.js" or "test/**/*Spec.js".
Enter empty string to move to the next question.
> js/*.js
21 08 2017 20:33:07.470:WARN [init]: There is no file matching this pattern.

> test/*Spec.js
21 08 2017 20:33:28.725:WARN [init]: There is no file matching this pattern.

>

Should any of the files included by the previous patterns be excluded ?
You can use glob patterns, eg. "**/*.swp".
Enter empty string to move to the next question.
>

Do you want Karma to watch all the files and run the tests on change ?
Press tab to list possible options.
> yes


Config file generated at ".../tdd/karma.conf.js".
```

5. Run the Karma Project with:
```bash
  karma start karma.conf.js
```
