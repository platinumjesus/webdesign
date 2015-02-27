# Chapter 3: Going Live

To publish your page, we'll use Github pages.

### [Create a Github account](github.com)

Avoid spaces and uppercase characters. Choose something short and simple with no spaces and uppercase characters, e.g. `jsmith` if your name is John Smith.

### Install the Github application (or git command line tool)

Download the Github app here:

[Mac OS](https://mac.github.com/)

[Windows](https://windows.github.com/)

If you're on GNU/Linux, just use your package manager to install the `git` package.

e.g. for Ubuntu: `sudo apt-get install git`

### Github app

#### Crete a new repository
Click the "+" button in the top left, and create a new repository. Call it yourname.github.io (it's very important that the name is exactly the same). This is the folder where you'll put your site's files later.

e.g. if your name is `jsmith`, call the repository `jsmith.github.io`

#### Create your website
Now you can get started working on your website in the repository folder.

#### Commit your work
Every once in a while it might be a good idea to save your progress. Git helps you with that, by making it easy to save snapshots of the current state of the project. You'll have to do this at least once to publish your site.

To commit your progress, you have to first add all the files for which you want to save your progress.

Then just commit them using an appropriate message describing the changes you made to the project, e.g. "changed the background color to blue".

#### Sync with Github
To push your site to Github and publish your site, just click the sync button in the top right. Now your website is live at yourname.github.io

You can just repeat this add-commit-push process every time you want to update your site.


### Command Line
First of all, kudos for using the command line!

### Create a new repository on Github
Create a new repository in the Github web interface. Call it yourname.github.io (it's very important that the name is exactly the same). This is the folder where you'll put your site's files later.

e.g. if your name is `jsmith`, call the repository `jsmith.github.io`

#### Clone the repository
From the command line, just type `git clone URL`, where URL is the repository URL you copied, e.g. `git clone https://github.com/bertob/webdesign`
To work in the repo, you have to `cd` into it, e.g. `cd webdesign`.

#### Create your website
Now you can get started working on your website in the repository folder.

#### Commit your work
Every once in a while it might be a good idea to save your progress. Git helps you with that, by making it easy to save snapshots of the current state of the project. You'll have to do this at least once to publish your site.

To commit your progress, you have to first add all the files for which you want to save your progress.
You can do this with `git add file1 file2 folder1`, e.g. `git add index.html style.css`

Then, you commit it with `git commit -m "description of changes you made"`, e.g. `git commit -m "changed the background color to blue"`.

#### Push to Github
To publish your site, just type `git push origin master`. This will copy your local version of the files to the server, and your site will be live at yourname.github.io.

You can just repeat this add-commit-push process every time you want to update your site.
