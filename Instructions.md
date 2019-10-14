## Introduction

## Step 0: Pre-event prepartion
### 0.1: Install git version control software
- Navigate to the [official git website](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and follow the instructions to download and install for your operating system
  - For Windows, use [this download link](https://git-scm.com/download/win) and install using all of the default (recommended) options.
### 0.2: Install and configure GitHub Desktop
- Navigate to [Github](https://github.com) and sign up for an account (if you don't already have one). 
- After registering, sign in to your account.
- Watch the short introductory video[What is GitHub?](https://www.youtube.com/watch?v=w3jLJU7DT5E).
- If using a Windows or Mac, download and install [GitHub Desktop](https://desktop.github.com/)
  - More guidance can be found in guides from [GitHub](https://help.github.com/en/desktop/getting-started-with-github-desktop) and [TechRepublic](https://www.techrepublic.com/article/how-to-install-github-desktop/).
  - Sign into GitHub Desktop using your GitHub credentials
  - In the *Configure Git* page, enter the name and email address that you want associated with your changes
  - In File > Options > Advanced, set the Shell to Git Bash
- (optional) Once configured, the main GitHub Desktop page will show any repositories that exist in your GitHub account. For those who use git already, you can add any local repositories that already exist on your machine.
### 0.3 Install Openrefine
- Navigate to [this setup page](https://datacarpentry.org/openrefine-socialsci/setup.html) and follow instructions for installing the Openrefine software. **NOTE** that you do not need to download the data file, as we'll be retrieving it in the workshop session using GitHub.

## Step 1: Forking a GitHub repository
In this step, you will 'fork' an existing (original) GitHub repository (belonging to someone else) to create a branch repository in your GitHub account. This allows you to create a copy of the original repository that you can modify as desired...and perhaps, allow your changes to be merged back 'upstream' to the original repository. 

- Ensure that you are logged into your GitHub account.
- Navigate to the workshop GitHub repository [https://github.com/data-curation/cdcf-workshop2A](https://github.com/data-curation/cdcf-workshop2A). 
- Click the **Fork** button at the top of the repository--this will "fork" the repository and create a branch in your GitHub account. By default, it will use a similar URL naming convention to the original (i.e. https://github.com/<yourUsername>/cdcf-workshop2A).

## Step 2: Clone to your local computer
In this next step, you will 'clone' your GitHub repository to your local computer so that you can work on files locally. 
**In GitHub Desktop:**
- Your newly forked repository should appear in the 'Your repositories' list in GitHub Desktop (You may need to refresh the list for it to show). 
  - **NOTE:** If it doesn't appear, double-check that the repository exists in your GitHub profile. If it does exist, you can copy the repository URL from GitHub and paste it into the appropriate place using the "Clone a repository from the Internet" button on GitHub Desktop.
- Highlight your repository in the list and click "Clone <*repository name*>". Select the local path where you would like to download the repository--a new folder will be created with the name of the repository. 
## Step 3: Do things in Openrefine!
- Once you've cloned the repository, use the button on GitHub Desktop to view the repository/files in Explorer. 
- Proceed with the [Data Carpentries Openrefine lesson](https://datacarpentry.org/openrefine-socialsci/01-introduction/index.html), using the downloaded data.
## Step 4: Export/Save modified data and processing script from Openrefine 
- Be sure to save all exported products (processing script, tar.gz project file, csv file) in the folder you cloned in Step 2.
## Step 5: Add and commit new files and changes to your local repository
- Maximize (or reopen) GitHub Desktop and open the local repository for this workshop (\cdcf-workshop2A). 
- The modified files will appear in the left-hand pane. Clicking on any of these files will display changes in the main pane.
- To commit changes, add a short summary (e.g. "outputs from OpenRefine workshop") and a further description of contents and activities (if desired). Click **Commit to master**.  
## Step 6: Push changes to your GitHub repository
- The repository overview page in GitHub Desktop will now display a new message: **Push 1 commit to the origin remote**. Click to push changes to the origin remote in GitHub. 
## Step 7: View and edit your readme file in the GitHub Editor
- Once your changes have been pushed to your remote (GitHub) repository, use your web browser to navigate to your GitHub repository. Confirm that the new files have been added to the repository along with the timestamp and summary from the commit.
- Explore the files in your GitHub repository. View the exported csv file, which will be presented in a formatted table. 
- View the README.md file and open it up for editing by clicking the pencil icon (*"Edit this file"*)
  - The README file is written in [Markdown](), a lightweight markup language that allows you to use plain text and a few special characters to create formatted text. 
  - More information and references for Markdown:
    - [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) 
    - [Adam Pritchard's Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
    - [Daring Fireball's Markdown Introduction](https://daringfireball.net/projects/markdown/)
- Edit the readme file to include pertinent information about the repository's creation, its contents, and sharing information. An empty template has been created for you from Cornell University's [Guide to writing "readme" style metadata](https://data.research.cornell.edu/content/readme). Click the **Preview changes** tab to see how the Markdown will render on the web.
- When finished editing, scroll to the bottom of the page, add a Summary and Description and commit changes to the master branch.
## Step 8: Pull GitHub changes to your local repository
- Maximize GitHub Desktop and click "Fetch origin" near the top of the window. A new prompt should appear to *"Pull 1 commit from the origin remote"*. Click **Pull origin** to incorporate the changes into your local repository. 
- Inspect the changes to your local repository.
## Step 9: Make a Pull Request to the original repository


## C. Introduction to [git](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) and Github
### C1. Setting up your git account ([git documentation](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)):
1. Set your name: ```git config --global user.name "John Doe"```
2. Set your email address: ```git config --global user.email johndoe@example.com```
3. Check your settings ```git config --list```

### C2. How git works
![alt text](https://git-scm.com/book/en/v2/images/lifecycle.png "git workflow")

### C3. Cloning a repository (from Github)
- Find a repository of interest on Github; Click the **Clone or download** button; Copy the url provided
- In git, navigate to the directory where you want to clone (download) the repository contents.
1. Clone the course repository: ```git clone https://github.com/3IE1/SciComp-2019.git``` (replace url for other repos)

### C4. Checking status, adding and committing changes
1. Create a new folder in the top directory (i.e. in /Sci-Comp2019/). Name it using your first initial and last name (no spaces)
2. In the new folder, **right click > create new file > text document**. Rename the file **readme.md**
- You have now created a markdown 'readme' file. 
3. Check the status of your repository (i.e. what's been modified): ```git status```
4. Add items to the list of tracked files (individually): ```git add <filename>```
- OR Add all items to this list of tracked files: ```git add --all```
5. Commit changes to git (i.e. record changes): ```git commit -m '<enter a note on what has changed>'```
- OR add and commit all at once: ```git commit -a -m '<enter a note on what has changed>'```
  
### C5. Push changes to a Github repository
- Ensure that you have permissions to write to the Github repository of interest (must be done in Github)
- Jay will have given you permission for the course repo.
1. Push changes to the target Github repository using the command: ```git push origin master```
- In this example -- which is the default case -- **origin** specifies the remote (i.e. Github) repository that is the target of your 'push'. **master** specifies the branch of the git repository that you're working on as the source data.
- To check if there are connected remote repositories use the command: ```git remote -v```

### C6. Pull changes 
- If others have pushed changes to the Github repository, you need to **pull** the changes to sync your local directory
- Pull changes: ```git pull origin master```
  - git **pull** actually runs two processes: **fetch** (get changes) and **merge** (place in your directory) 
- You can check changes (before merging them) with: ```git fetch``` ```git diff origin master```

### C7. More information
- [Official git documentation page](https://git-scm.com/book/en/v2/)
- [The Smart Ways to Correct Mistakes in Git](https://css-tricks.com/the-smart-ways-to-correct-mistakes-in-git/) 

## D. An introduction to Markdown
### D1. What is Markdown? 
Borrowed shamelessly from Github's [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) page: 
> Markdown is a way to style text on the web. You control the display of the document; formatting words as bold or italic, adding images, and creating lists are just a few of the things we can do with Markdown. Mostly, Markdown is just regular text with a few non-alphabetic characters thrown in, like # or *.

Markdown uses simple notation to apply simple formatting rules. Since it's pretty much just plain text, it's transferrable and much simpler than marked-up text like HTML or even Word or Google documents. For much of the writing that you do for the web, Markdown is good enough. Github uses Markdown for its documents (this document was created in markdown), as does a variety of other web platforms (Trello, for example). 

Using Markdown in Github lets you create readme files that can use better formatting than a plain text file, but is still readable as plain text -- it's the best of both worlds. 

### D2. Get familiar with Markdown
1. Using the Github web interface, add some content to your newly-created **readme.md** document. Use the [Mastering Markdown guide](https://guides.github.com/features/mastering-markdown/) as a reference (or other guides on the web) to create a fictional document that contains the following elements: 
- Headings of a number of different levels
- bolded, italicized text 
- insert an image from the web
- An ordered list
- A bulleted list
- A link to another website 
- A table
- And finally, an emoji! 
2. Commit your changes and enjoy the products of your hard work!


### Configuring Github desktop
- Install Github desktop 
- Once installed, click the gear button and select **Options**
  - Under *Accounts*, add your GitHub account 
  - Under *Configure git*, add the name and email address that you want associated with your changes
  - Under *Clone path*, enter the path to the default directory where you would like to create or clone repositories (e.g. D:\Local). If you have existing repositories in the default directory, cick *Scan for Repositories*. 
  - In Default shell, select **Git Bash** for the purposes of this tutorial.

Notes 

When a repo is cloned, it has a default remote called origin that points to your fork on GitHub, not the original repo it was forked from
[What is Github?](https://www.youtube.com/watch?v=w3jLJU7DT5E)
OpenRefine is an open source project that is developed in a [github repository](https://github.com/OpenRefine/OpenRefine). 
[Installing GitHub Desktop](https://www.techrepublic.com/article/how-to-install-github-desktop/)

We're all working on 
