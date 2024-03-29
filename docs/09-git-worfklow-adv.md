
# Making a Pull Request -- Advanced

## Prerequisites

- [Have an understanding of why Github is useful](https://hutchdatascience.org/dasl-snack-github/why-github.html)
- [Have a GitHub account](https://hutchdatascience.org/dasl-snack-github/create-a-github-account.html)
- [Create a repository on Github](https://hutchdatascience.org/dasl-snack-github/setting-up-a-project-on-github.html)
- [Set up a Git Client](https://hutchdatascience.org/dasl-snack-github/setting-up-a-git-client.html)

## Set up a Git Client (GitKraken)

Interaction with git and GitHub can be done completely from the command line, but sometimes this can be harder to keep track of. To help us navigate this, we recommend using a git client. There are a lot of different clients out there, and they are generally free for most situations you will need. In this course, we will take you through how to use [GitKraken](https://www.gitkraken.com/git-client), one such git client.

GitKraken is nice because they have lots of nice tutorials, it works pretty well, and its free for most use cases. But if you find GitKraken doesn't work for you, you can explore [other git clients](https://www.hostinger.com/tutorials/best-git-gui-clients/). For this course, we'll be using GitKraken.

### Install GitKraken

[Go here to install GitKraken](https://support.gitkraken.com/how-to-install/).

Follow their instructions to sign in with your GitHub account. It will ask you to authorize your GitHub account to connect to GitKraken. Click `Authorize`.

You may find it helpful to watch GitKraken's own tutorial (linked below) about how to "git" started, but we will also guide you through each step!

<iframe src="https://www.youtube.com/embed/ub9GfRziCtU" width="672" height="400px"></iframe>

GitHub has a host of terms that can feel like a whole language at first, but we'll introduce them one at a time. To start, a lot of the GitHub workflow centers around handling copies of your code that are either stored on the internet (are _remote_) or are stored on your computer (are _local_).

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_120.png" title="GitHub has a whole host of terms that can feel like a whole language at first, but we'll introduce them one at a time. To start with, a lot of the GitHub workflow centers around handling copies of your code that are either stored on the internet (are _remote_) or are stored on your computer (are _local_)." alt="GitHub has a whole host of terms that can feel like a whole language at first, but we'll introduce them one at a time. To start with, a lot of the GitHub workflow centers around handling copies of your code that are either stored on the internet (are _remote_) or are stored on your computer (are _local_)." width="100%" />
<div class = "github">
**Remote** = GitHub on the internet <br>
**Local** = What's on your own computer
</div>

A _repository_, in the case of a data science project, is mostly synonymous with the word "project". Using GitHub, a project will exist both as a remote repository and a local repository (in other words, it will be on the internet on GitHub and on your computer).

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_149.png" title="A remote repository is project that is stored on the internet for example, a URL to jhudsl/reproducible-R-example. A local repository is a project copy that lives on your computer. For example, a file path to reproducible-R-example. So using GitHub, a project will exist both as a remote repository and a local repository. (It will be on the internet on GitHub and on your computer). " alt="A remote repository is project that is stored on the internet for example, a URL to jhudsl/reproducible-R-example. A local repository is a project copy that lives on your computer. For example, a file path to reproducible-R-example. So using GitHub, a project will exist both as a remote repository and a local repository. (It will be on the internet on GitHub and on your computer). " width="100%" />

<div class = "github">
**Repository** = a set of project files that have a location on GitHub
</div>

## Start a GitHub repository

If you don't already have a Github repository in mind that you are working from, you can create one using these steps:

- Go to [Github's main page](https://github.com/) and sign in with your GitHub account.
- Follow [these instructions to create a repository](https://docs.github.com/en/get-started/quickstart/create-a-repo). As a general, but not absolute rule, you will want to keep one GitHub repository for one analysis project.
  - Name the repository something that reminds you what its related to. For these examples, we're calling using `repository-name` as our placeholder.
  - Choose `Public`.
  - Choose `add a README`.
- Follow [these instructions](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository#adding-a-file-to-a-repository-on-github) to add your files to this repository.

This new repository you created should look [something like this](https://github.com/cansavvy/repository-name).

### git clone

Now you have a repository on GitHub online!

In our daily grind, we will work on this code from our own computer. To set this up, we'll need to `clone` it to our own computer. Cloning is making a remote copy of the project local.

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_90.png" title="To clone a repository means to copy a remote repository to your local computer" alt="To clone a repository means to copy a remote repository to your local computer" width="100%" />

<div class = "github">
**clone** = To make a remote repository local. In other words, to make an online repository downloaded and linked on your computer.
</div>

To get started, you will need to clone the GitHub repository you created. We will be using this repository for the duration of this course.

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_166.png" title="To clone a GitHub repository, using GitKraken. First, Click Clone a repo. Then, choose where you’d like the repository to be on your computer using the ‘Browse’ button. Then Copy + Paste the url to the project you want to clone where it says ‘URL’. Then click `Clone the repository’." alt="To clone a GitHub repository, using GitKraken. First, Click Clone a repo. Then, choose where you’d like the repository to be on your computer using the ‘Browse’ button. Then Copy + Paste the url to the project you want to clone where it says ‘URL’. Then click `Clone the repository’." width="100%" />

It is simple to clone a GitHub repository using GitKraken. First, sign in to GitKraken; under Repository Management > Clone tab, click `Clone a repo`. Then, choose where you’d like the repository to be on your computer using the `Browse` button. You will need to `Copy + Paste` your new repository's URL (web address) to  where it says `URL`.

Navigate to your repository on GitHub to copy the URL. Copying and pasting is advisable because any little typo will inhibit cloning.

Now you are ready to click `Clone the repository`! It will ask you if you'd like to `Open Now`, click that.

### Create a branch

Handling branches is where you unleash the real benefit of GitHub, but it's also the confusing part to get the hang of.

<div class = "github">
**branch** = a unique working copy of file changes of a GitHub repository. A branch can be local and remote.
</div>

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_266.png" title="Using branches is where you unleash the real benefit of GitHub, but it's also the confusing part to get a hang of. Currently, the repository we just made has a main branch. The main branch is the default branch and is The main branch is what you want most curated, working, and always ready for others to use!" alt="Using branches is where you unleash the real benefit of GitHub, but it's also the confusing part to get a hang of. Currently, the repository we just made has a main branch. The main branch is the default branch and is The main branch is what you want most curated, working, and always ready for others to use!" width="100%" />

The best way to get a grasp on what the branches represent is to create one and start using it.

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_632.png" title="In GitKraken we can create a new branch; this will be your working copy. First, click the Branch button. Next, type in a branch name in the box that the cursor is blinking in. In our example, we are calling it a-new-branch. Then click Enter! Now you have a new branch!" alt="In GitKraken we can create a new branch; this will be your working copy. First, click the Branch button. Next, type in a branch name in the box that the cursor is blinking in. In our example, we are calling it a-new-branch. Then click Enter! Now you have a new branch!" width="100%" />

In GitKraken we can create a new branch; this will be your working copy. First, click the Branch button. Next, type in a branch name in the box that the cursor is blinking in. In our example, we are calling it `a-new-branch`. Now click `Enter`! Now you have a new branch!

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_618.png" title="Now that we’ve created this new branch, we can do what we like with a-new-branch, knowing that main will remain safe." alt="Now that we’ve created this new branch, we can do what we like with a-new-branch, knowing that main will remain safe." width="100%" />

Now we can edit our files and code however we normally would. Go ahead and make an edit to any file in your new repository.

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_645.png" title="Now that we are on our new branch, we will Edit a file as you normally would). Make any change to the README.md file in your local repository. Save the changes you make to that file. Now the changes you make to any files in this repository should show up here." alt="Now that we are on our new branch, we will Edit a file as you normally would). Make any change to the README.md file in your local repository. Save the changes you make to that file. Now the changes you make to any files in this repository should show up here." width="100%" />

If you've made a change to any file in your repository, it will appear in GitKraken and you can click on it to see the differences.

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_652.png" title="To see how the file is different, click on the filename in the right side of the GitKraken screen. To add the file to the staged change, click on the Stage File button. " alt="To see how the file is different, click on the filename in the right side of the GitKraken screen. To add the file to the staged change, click on the Stage File button. " width="100%" />

If we want to add these file changes to our current branch, we need to `commit` them.

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_664.png" title="To commit files is to include your set of file changes to your current branch. Write a commit message that explains the changes. Now click on the button that says Commit changes to 1 file." alt="To commit files is to include your set of file changes to your current branch. Write a commit message that explains the changes. Now click on the button that says Commit changes to 1 file." width="100%" />
<div class = "github">
**add** = to stage your files to be committed to your current branch. <br>
**commit** = include your set of file changes to your current branch.
</div>

Now that we have changes committed to our branch we are ready to add them to the remote, internet copy! To do this, we will need to `push` our branch.

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_686.png" title="To push changes on GitHub means to add changes to the remote repository on GitHub." alt="To push changes on GitHub means to add changes to the remote repository on GitHub." width="100%" />

To push means to add changes that are on your new branch to the remote branch (internet version). You can select your _origin_, which refers to where your branch is stored on the internet. Choose your origin in the dropdown menu and click Submit.

<div class = "github">
**origin** = where your branch is stored on the internet (remotely)
**push** = to add changes from your branch to its remote counterpart. In other words, put your changes online.
</div>

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_786.png" title="To push means to add changes that are on your new branch to the remote branch (internet version). The word origin just refers to where your branch is stored on the internet. Choose your origin in the dropdown menu and click Submit. " alt="To push means to add changes that are on your new branch to the remote branch (internet version). The word origin just refers to where your branch is stored on the internet. Choose your origin in the dropdown menu and click Submit. " width="100%" />

After a variable number of commits, your branch, called `a-new-branch`, is a different version of the original code base that may have a nifty improvement to it. But our main goal is to add that nifty improvement to the main branch. To start this process of bringing in new changes to the main curated repository, we will create a `pull request`.

<div class = "github">
**pull request** = A way to propose changes from a branch to be included into the main repository.
<br>
From GitHub:
> Pull requests let you tell others about changes you've pushed to a GitHub repository. Once a pull request is sent, interested parties can review the set of changes, discuss potential modifications, and even push follow-up commits if necessary.

</div>

Pull requests are the meat of how code changes and improvements get reviewed and incorporated! A vast majority of the benefits of incorporating GitHub into your workflow centers around fully utilizing the power of pull requests!

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_751.png" title="After a variable number of commits, your branch, called a-new-branch is a different version of the original code base that may have a nifty improvement to it. But our main goal is to add that nifty improvement to the main branch. To start this process of bringing in new changes to the main curated repository, we will create a pull request. A pull request will show us the difference between main and a-new-branch so you scrutinize this feature before adding it to the main branch." alt="After a variable number of commits, your branch, called a-new-branch is a different version of the original code base that may have a nifty improvement to it. But our main goal is to add that nifty improvement to the main branch. To start this process of bringing in new changes to the main curated repository, we will create a pull request. A pull request will show us the difference between main and a-new-branch so you scrutinize this feature before adding it to the main branch." width="100%" />

Now we can open up a pull request if we go to our GitHub repository on GitHub.

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_713.png" title="If we’ve recently pushed our changes, we can go to our repository on GitHub and a yellow banner will prompt us to start a new pull request. " alt="If we’ve recently pushed our changes, we can go to our repository on GitHub and a yellow banner will prompt us to start a new pull request. " width="100%" />

After you click on `Compare & pull request` you'll be taken to a screen where you can add information about your changes. After you are done writing your description, click `Create Pull Request`! (If you don't have your pull request description _perfect_ don't worry about it, you can always edit it later).

Congrats! You've just opened a pull request!

In an upcoming chapter we will discuss what information you should put in this pull request description to make it pertinent for yourself and whoever reviews your pull request.

To summarize, below is what this workflow looks like:

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g1014c75158f_0_675.png" title="An overview of the GitHub workflow. Uploaded a project to GitHub. Clone that project to your computer. You will only have to do this cloning and set up step once per repository/project. Now let’s say you have an update in mind. Make a new branch to work off of. Edit code as you normally would. Add and commit the file changes to your branch. Push the changes to your remote branch. Repeat these steps until it you’ve addressed the update you had in mind Now, Create a pull request." alt="An overview of the GitHub workflow. Uploaded a project to GitHub. Clone that project to your computer. You will only have to do this cloning and set up step once per repository/project. Now let’s say you have an update in mind. Make a new branch to work off of. Edit code as you normally would. Add and commit the file changes to your branch. Push the changes to your remote branch. Repeat these steps until it you’ve addressed the update you had in mind Now, Create a pull request." width="100%" />

One more note: if you do want to use the command line or if you want to know more about the specific git commands that GitKraken is doing for you (which might be handy for troubleshooting), **the specific commands that can be used or Googled at each step are highlighted in red in the images** - you just need to add `git` before them! For example, you would type `git push` in your command line in order to push your code. Or if you'd like to know more about pushing code, you can google `git push`.

<img src="09-git-worfklow-adv_files/figure-html//1IJ_uFxJud7OdIAr6p8ZOzvYs-SGDqa7g4cUHtUld03I_g122da391674_0_5.png" title="Alternative text" alt="Alternative text" width="1250" />

## More resources for learning GitHub

- [Happy Git and GitHub for the useR](https://happygitwithr.com/) by @Bryan2021.
- [GitHub for data scientists](https://towardsdatascience.com/introduction-to-github-for-data-scientists-2cf8b9b25fba) by @Vickery2019.
- [GitHub docs about creating a Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) by @GitHub2021b.
- [Making a Pull Request](https://www.atlassian.com/git/tutorials/making-a-pull-request) by @Radigan2021.


**If you have any feedback on this chapter, please [fill out this form](https://forms.gle/j3cJZX5CmNtQp6QKA), we'd love to hear your feedback!**
