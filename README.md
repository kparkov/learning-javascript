# Learning JavaScript

## Preparations

- [ ] Make sure that you have a Github account. If not, create one.
- [ ] Create a new repository in Github. Make it your own "learning javascript" repository. Make it public.

## Software installs

- [ ] Install [Chocolatey](https://chocolatey.org/). Chocolatey is a package manager for Windows, and will make it easy to install software.
- [ ] Install Microsoft Windows Terminal using Chocolatey. Note that you need to start the terminal as Administrator to run Chocolatey commands.
- [ ] Check that `git` is installed in the terminal. If it isn't, install it using Chocolatey.
- [ ] Install Node.js if it is not already installed.
- [ ] Install Visual Studio Code if it is not already installed.

## Introduction to `git`

- [ ] Clone your learning repository (this repository) onto your computer.
- [ ] Open the local folder in Visual Studio Code.

Your "learning javascript" repository is for all exercises related to this project. Each exercise / code project will be put in a separate subfolder. In the top of the repository, we will put a `README.md` file. This will be the text that is on the front page of the online repository, and is typically used for:

- A description of what the repository contains or what the code does.
- Instructions on how to download and install the code.
- Instructions on how to use the code.

Tasks:

- [ ] Add a `README.md` file with a paragraph of meaningful text. in your local copy of the repository using Visual Studio Code.
- [ ] Go into source control in Visual Studio Code and see that your changes are registered. Make a commit. Be sure to provide a meaningful title.
- [ ] Push the changes to the remote (Github) using the <kbd>Sync</kbd> button in VS Code. This can always be used to sync changes from and to the remote. Go to the webpage and confirm that the changes have been pushed correctly.
- [ ] Add a `.gitignore` file in the root. The contents of the file is shown on this url: http://www.gitignore.io/api/node
- [ ] Commit the `.gitignore` file providing a meaningful message, and sync it to the remote.

## First JS project

- [ ] Create a subfolder in the repository root for your first code project.
- [ ] From a terminal, use `npm init` inside that subfolder to create a new project. If done correctly, the subfolder will now contain a single file called `package.json`.
- [ ] Create a first project that will output some text of your own choice to the screen.

## Code lessons

- `console.log`
- `let` / `const`
- data types: `string`, `number`, `boolean`, `array`, `object`, `undefined` and `function`. We also have `bigint` and `symbol` for later lessons. Finally, we have `null` as a special value, but it is of type `object`.