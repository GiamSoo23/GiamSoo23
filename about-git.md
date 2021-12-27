# About Git

If you don't know much about computers or programming, you may not know git either. Today I'm going to explain (at least what I've learned or remebered) about it.

## What is git?

Git is a tool that is used to track changes among different files, usually programming projects. It runs on your computer, and it is usually paired with online git services, such as github, that allow you share code changes with a team.

## How do I use git?

1. Install [git](https://git-scm.com/) on your computer. This will allow you to use git commands.
2. Open a terminal on the folder where your project will be. There, run `git init`. This creates a new repository starting on the `main` branch.
3. Now you are allowed to create your first commit! But first you should create any type of document and make any change. Then use the command `git add`, followed by the files you want to commit, to prepare your commit.
4. After setting up the files to commit, run `git commit -m "MESSAGE"`, where MESSAGE is a short text describing the commit.
5. With an account on a website like github, create a repository and follow the instructions to connect your local repository to the remote repository.
6. To upload new commits to the cloud, use `git push`. Also use `git pull` to get any new commits!

With these few steps you will be able to start a repository!

You are excited, don't you? See you in the next tutorial :D
