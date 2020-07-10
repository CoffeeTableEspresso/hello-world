# hello-world
# Welcome! Come learn about Git and Github.

Git/Github can seem intimidating at first, but don't worry! There is a steep learning curve, but once you get the hang of it, it is useful for programming. Use this guide as one of your resources and you'll be on your way to mastering Git/Github! 

## What is Git and Github? What's the difference between them?

## Git

Before you understand what Git is, you'll need to understand what is a version code and control system. 

Here's how [atlassian](https://www.atlassian.com/git/tutorials/what-is-version-control) explains version code: 

> Git is a software available for you to manage changes to your code over time. Version control software keeps track of every modification to the code in a special database. If a mistake is made, developers can turn back the clock and compare earlier versions of the code to help fix the mistake"

It can be considered like your history on your search engine. It allows you to see the progress and what you've done! [maybe a better analogy?]

> Git is the most widely used modern version control system in the world.

The same website explains ["What is Git"](https://www.atlassian.com/git/tutorials/what-is-git)

Here are some main points from the article: 

- Why do we use Git?
    - It is the most widely used modern version control system in the world.
        - This is important because that means that if you collaborate with other developers, you'll be able to work within the same system.
- Compared to other alternatives, Git has the **performance, security, flexibility** that most teams and individuals need. It's the most broadly adopted tool of its kind, which makes that many individuals use it and third party software tools and services are already integrated with Git.

More questions? Check out the full article [here](https://www.atlassian.com/git/tutorials/what-is-git)!

### GitHub

GitHub can be considered a code sharing and publishing service or a social networking site for programmers. 

**Code sharing and publishing service** 

[Techcrunch](https://techcrunch.com/2012/07/14/what-exactly-is-github-anyway/) describes GitHub as "filing system for every draft of an document".

One of GitHub's best functions is the ability to copy code from another user's account to another. You're able to take a project that you didn't make and modify it under your own account. 

Techcrunch describes GitHub as:

> The flagship functionality of GitHub is “forking” – copying a repository (the main "folder" where the code is stored) from one user’s account to another. This enables you to take a project that you don’t have write access to and modify it under your own account. If you make changes you’d like to share, you can send a notification called a “pull request” to the original owner. That user can then, with a click of a button, merge the changes found in your repository  with the original repository.
These three features – fork, pull request and merge – are what make GitHub so powerful.

Before GitHub, you would have to manually download the project's source code, make changes on your own computer and then create a "patch" - which holds your changes and email the patch to the project's head programmer. Then, they would have to evaluate the patch and decide whether to add your changes to the original project. 

**Networking**

GitHub stores all your code where other people can see what you've written and your contributions to other projects. It's like a resume for your code. If your match is accepted, you're able to get credit on the original project, which shows up on your profile. 

More questions? Check out the full article [here](https://techcrunch.com/2012/07/14/what-exactly-is-github-anyway/)!

These are the basic concepts behind Git and GitHub. Learn more by going to the Git and GitHub resources!

# Git Workflow & Common Pitfalls/Mistakes

## **git workflow**

1. (first time setup) pull the repository `git clone https://github.com/dryu99/infinite-animal-crossing-lofi.git`
    - what does pulling the repository mean?
        - you're "grabbing" the latest version of the code from GitHub
        - you only need to do this once at the beginning
        - this is what it could look like

        ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3e1c36dc-0a94-4f25-a2f1-4bb15329f788/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3e1c36dc-0a94-4f25-a2f1-4bb15329f788/Untitled.png)

2. checkout into a new branch `git checkout -b NAME-OF-BRANCH`
    - it should look like this:
        - the name of the **original** branch is called (CREDITSS) - shown in a blue color
            - if you start out for the first time, the branch will be called MASTER/MAIN
        - we checked out to a new branch called EXAMPLE

    ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f5d737ce-7adf-45b1-830b-5db68c7dd79d/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f5d737ce-7adf-45b1-830b-5db68c7dd79d/Untitled.png)

    - checking out into a new branch means that you're working on a different version
        - like a paper - this means you're working on a draft involving one idea for the final paper
        - you don't want to work on the idea directly on the final paper but rather on a draft
        - if you don't use the "draft" having branches makes it easier to not include it
        - if you do use the "draft" you can easily put it in the final paper - master
3. make your changes, go wild!
    - you can add something to the README or add text
4. tell git to track your changes by doing `git add .`
    - you can do this before you start or afterwards
5. save your changes and give it a meaningful name by doing `git commit -m "describe your changes here"`
6. double check to see what git is keeping track of by doing `git status`
7. push those changes up to github `git push origin NAME-OF-BRANCH`
8. go to github and make a pull request!
9. merge it into master branch 

## Common Pitfalls/Mistakes

### **common pitfalls**

1. help! what do i do if my git says "failed to push some refs to origin"
    1. you wanna pull your changes and do `git pull origin master`
2. help! i wanna revert to an earlier version!
    1. find the last time you saved your work by doing `git log` and keep track of the hash
    2. then `git reset --hard <hash>`
3. how do i update my local version to be up to date with github?
    1. `git pull origin master`
4. how do i switch branches?
    1. `git checkout NAME-OF-BRANCH`

### common mistakes

- not including spaces between your commands `gitcommit` vs `git commit`
- not pushing or pulling your repository
    - not pulling -this means that you aren't working on the latest version of the project
    - not pushing - that means you haven't uploaded the latest version of the project
- working on the wrong branch
    - you meant to do it in branch A but you did it in branch B
    - check which branch you're on in git
- working on the master directly (if there are multiple people working or different versions)
    - similarly to a paper, it would be as if you're working on the final paper rather than a draft
    
    
    # Resources

Here's a list of resources to use to learn more about Git/GitHub!

[GitHub's guide to setting up - Hello World](https://guides.github.com/activities/hello-world/)

Official GitHub Handbook

[Copy of official git handbook](https://www.notion.so/Copy-of-official-git-handbook-a1b0638c198a4b75bce8605e7baf0662)
- [What is GitHub? - GitHub](https://youtu.be/w3jLJU7DT5E)
- [Git Branching](https://learngitbranching.js.org)
- [Basic Git Commands](https://dev.to/dhruv/essential-git-commands-every-developer-should-know-2fl)
- [**An Intro to Git and GitHub for Beginners (Tutorial)](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)** by Meghan Nelson
- [https://learngitbranching.js.org](https://learngitbranching.js.org/)
- [git - the simple guide](https://rogerdudler.github.io/git-guide/)
- [Learn the Basics of Git in Under 10 Minutes](https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/)
- [Git: Become an Expert in Git & GitHub in 4 Hours (Udemy Free Course)](https://www.udemy.com/course/git-expert-4-hours/)
- [A Visual Git Reference](http://marklodato.github.io/visual-git-guide/index-en.html)

    [git workshop.pdf](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f6f38021-2ee8-4e8c-8f3e-01ad80d6142b/git_workshop.pdf)


