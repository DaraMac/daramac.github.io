# Introduction
- By the end of this workshop, all your code will be safely backed up, and always will be, and done easily from now on.
- We will mostly focus on solo, but touch on collaboration.
- What is version control and why should you do it?
    - A way of backing up, and also versioning any text.
    - A free and fairly easy and quick way to ensure you **don't ever lose your code**.
    - Also keeps track of versions, no more **FINAL, LAST EDIT, COPY**
    - Share and collaborate more easily
    - Keep everything in one place
- What should you version control?
    - Everything text
        - Code
        - Papers (if not already on Overleaf)
        - Latex presentations
        - Notes
    - Datasets?
        - Possibly not pure text, so not such a good fit for VCS like git
        - Maybe too big
        - But some will be appropriate
        - Should be backed up _somewhere_!
- Why git?
    - It's just the biggest, most popular and thus well supported and resourced version control system.
    - No more "FINAL (2)" "MAY-23_04v2"
    - [Github](https://github.com) and (Maynooth) [Gitlab](https://gitlab.cs.nuim.ie) if you're a CS student.
    - Can also follow and discover interesting projects there.

# Getting started
## Installation
- Install the [command line tool](https://git-scm.com/downloads).
- ssh-keys!
- Don't worry we'll get to [GUIs](https://git-scm.com/downloads/guis) later
    - And [editor integration](https://code.visualstudio.com/docs/sourcecontrol/overview).
- But first let's learn the basics: by backing up our own code.
- We'll walk through it, and learn the key git concepts as we go.

# Resources
- [Cheat sheet](https://training.github.com/downloads/github-git-cheat-sheet.pdf) from Github.
- [Juliva Evans cheatsheet](https://wizardzines.com/git-cheat-sheet.pdf)
- [Oh shit, git!](https://wizardzines.com/zines/oh-shit-git), by Julia Evans, might be worth buying this and printing it out for everyone!
    - She's working on another Git zine on its terminology.
- [Git in six hundred words](https://maryrosecook.com/blog/post/git-in-six-hundred-words)
    - [Git from the inside out](https://maryrosecook.com/blog/post/git-from-the-inside-out), more detailed version.
- [Pro Git](https://git-scm.com/book/en/v2), for Pros.
    - Even reading through a few sections now and then will be helpful.
- [So You Think you know Git](https://www.youtube.com/watch?v=aolI_Rz0ZqY), I want to check this out
- [Game](https://ohmygit.org)
- [Software Carpentry](https://swcarpentry.github.io)

# Questions
- Is your code backed up?
    - Yes: 4, RServer: 1, Github: 5, Overleaf: 3
    - No: 1
    - If yes how? How often?
        - Daily: 5
        - Yearly: 1
- What do you code in?
    - RStudio: 4
    - VSCode: 3
    - Jupyter Notebook: 1
    - JCreator: 1
    - Visual Studio 2019: 1
    - PyCharm: 1
    - Notepad++: 1
    - Spyder: 0 (Conor says he should try)
    - Processing: 1

# Common Problems
- Large file storage
    - What it is, when to use it, how to remove broken things
    - [BFG](https://rtyley.github.io/bfg-repo-cleaner)
- Would like to do it automatically, no typing in terminal
- Stash
- Collaboration
- Don't back up .Renviron, from [here](https://bookdown.org/content/d1e53ac9-28ce-472f-bc2c-f499f18264a3/envManagement.html#use-.renviron-file)

# Reproducibility
- Personal
    - I want you to ask yourself, how long would it take to restore all your work on a brand new machine, and how difficult/easy would it be?
    - No need for hypothetical, let's test right now!  (maybe on a blank VM I set up)
- For other researchers / users
