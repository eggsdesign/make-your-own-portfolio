# Day 1: Putting a page up on the internet

## 1. Create a repository on GitHub

<details>
	<summary>Show me</summary>

![Create repo](./assets/create-repo.gif)

</details>

To make hosting simpler, follow these steps closely

1. Make sure you are logged in to GitHub. Click the GitHub logo to navigate to the front page.
2. Click on the `New` button to create a new repository.
3. Name it `<username>.github.io`. In my case, the repo is called `avanvik.github.io` This will make hosting with GitHub Pages work almost like magic ✨
4. Click `Create repository`
5. **Important** Click `HTTPS`and copy the generated repo link (mine looks like this`https://github.com/avanvik/avanvik.github.io.git`
6. In VSCode, click `clone repository...` and paste in the GitHub repo url. Pick where you want to put the project. I usually put mine in `Documents/Projects/`. **Note:** VSCode will try to authenticate your GitHub user, so just follow the required steps for that.

<details>
	<summary>Show me</summary>

![Clone repo](./assets/clone-repo.gif)

</details>

## 2. Create a 'main' branch

A git branch is like a folder where your code changes go. GitHub Pages require a `main` branch, but VSCode – for some dumb reason – starts with a `master` branch. Solve this by creating a new branch in VSCode.

1. In the VSCode toolbar (the bar stuck to the top of your screen on Mac) click `Terminal > New Terminal`. This will open a new panel with a terminal in it, navigated to your project folder.
2. Type `git checkout -b main` and click Enter to run the command. This will create a new branch called `main` and set it as the active branch.

<details>
	<summary>Show me</summary>

![Open terminal](./assets/new-terminal.png)

</details>

## 3. Create an HTML file

1. In VSCode, create a new file in your project folder.
2. Name it `index.html` and open the file.
3. Add `<h1>It works!</h1>` to the html file and save it.

Your index.html file should look like this now:

```html
<h1>It works!</h1>
```

## 4. Commit your changes

<details>
	<summary>Show me</summary>

![Commit changes GIF](./assets/add-and-commit.gif)

</details>

1. In VSCode click the "Source Control" tab in the left sidebar. It should have a notification icon, since you added your index.html file.
2. Click the "✔" Icon to commit all changes
3. Click the arrow icon to push your changes to GitHub (Lower left corner of the editor window).

**Note:** For some people this might trigger an error message, saying that github username and email are not properly configured.

To fix this, run the following commands – one by one – in your terminal in VSCode. Replace the parameters in "" to contain your own name and e-mail, and click Enter to run each command.

```
git config --global user.name "Your Name"
git config --global user.email "youremail@yourdomain.com"
```

<details>
	<summary>Show me</summary>

![Fix git in terminal](./assets/terminal.png)

</details>

## 5. Add more HTML content

HTML is all about structure and content! But not about style (that is where CSS comes in). Almost all HTML documents follow this basic structure:

```html
<!DOCTYPE html>
<html>
  <!-- Meta data goes in the <head> -->
  <head>
    <title>Title of page</title>
  </head>

  <!-- Content goes in the <body> -->
  <body>
    <h1>Welcome to Alexanders portfolio</h1>
    <p>I do pixels and code, and occasionally give talks on conferences</p>
  </body>
</html>
```

**When you are done** with adding content to your html page, do the following to update your GitHub Pages-hosted website:

1. Save the HTML file
2. Commit the changes
3. Push to GitHub
