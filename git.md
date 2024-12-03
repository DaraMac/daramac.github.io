# Introduction
- By the end of this workshop, all your code will be backed up, and be done easily and continually from now on
- We will mostly focus on solo work, but touch on collaboration

## What is version control and why should you do it?
- A way of backing up, and also versioning any text
- A free and fairly easy and quick way to ensure you **don't ever lose your code**
- Also keeps track of versions, no more **FINAL, FINAL (2), LAST EDIT, COPYv2**
- Share and collaborate more easily
- Reproducibility
- Keep everything organised in one place

## What should you version control?
- Everything text
    - Code
    - Papers (if not already on Overleaf)
    - Latex presentations
    - Notes
    - Configuration files (dotfiles)
- Datasets?
    - A small to mid size csv maybe
    - Possibly not pure text, so not such a good fit for VCS like git
    - Maybe too big
    - But some will be appropriate
    - Should be backed up _somewhere_!
    - Can touch on this later

##  Why git?
- It's just the biggest, most popular and thus well supported and resourced version control system

## Fun Things!
- GitHub pages site
    - [My site](https://macconville.ie)
        - [Repo](https://github.com/DaraMac/daramac.github.io)
    - [Cormac's site](https://c-monaghan.github.io)
- Or simpler, a personal README.md
- [Cormac again](https://github.com/C-Monaghan)
- Social network features
    - Stars
    - Following

# Reproducibility
- Personal
    - I want you to ask yourself, how long would it take to restore all your work on a brand new machine, and how difficult/easy would it be?
    - No need for hypothetical, let's test right now!  (maybe on a blank VM I set up)
- For other researchers / users
- Licence!
- Demo

# Questions
- What do you code in?
    - RStudio:          0
    - VSCode:           0
    - Jupyter Notebook: 0
- Is your code backed up?
    - Yes: 0
        - RServer:  0
        - Github:   0
        - Overleaf: 0
    - No: 0
    - If yes how? How often?
        - Daily:   0
        - Weekly:  0
        - Monthly: 0
        - Yearly:  0

# Resources
- [Official website](https://git-scm.com)
- [Pro Git book](https://git-scm.com/book/en/v2), for Pros
    - Even reading through a few sections now and then will be helpful
- Cheat Sheets
    - [Julia Evans](https://wizardzines.com/git-cheat-sheet.pdf)
    - [GitHub](https://training.github.com/downloads/github-git-cheat-sheet.pdf)
    - [Visual](https://ndpsoftware.com/git-cheatsheet.html)
- [happygitwithr.com](https://happygitwithr.com)
- [The Turing Way on Version Control](https://book.the-turing-way.org/reproducible-research/vcs), but also the whole book
- [learngitbranching.js.org](https://learngitbranching.js.org)
- [Oh Shit, Git!?! website](https://ohshitgit.com)
    - [zine](https://wizardzines.com/zines/oh-shit-git), she is working on another zine
- [Oh My Git game](https://ohmygit.org)
- [Software Carpentry lesson](https://swcarpentry.github.io/git-novice)
- [So You Think you know Git video](https://www.youtube.com/watch?v=aolI_Rz0ZqY)
- [Git in six hundred words](https://maryrosecook.com/blog/post/git-in-six-hundred-words)
    - [Git from the inside out](https://maryrosecook.com/blog/post/git-from-the-inside-out), more detailed version

# Installing
## CLI
- Install [git](https://git-scm.com/downloads), a CLI
- I use this but with modifications (shell add-ons, aliases, ask me if interested!)
- Let's learn the basics: by backing up our own code
- We'll walk through it, and learn the key git concepts as we go

## GUIs
- These are standalone GUIs, not integrated into an editor
- [Official list](https://git-scm.com/downloads/guis)
- [GitHub Desktop](https://github.com/apps/desktop), for Mac and Windows
- [GitUp](https://github.com/git-up/GitUp), Mac only, Julia Evans recommendation
- [Gitnuro](https://gitnuro.com), all platforms
- [SourceGit](https://github.com/sourcegit-scm/sourcegit), all platforms
- [Gittyup](https://murmele.github.io/Gittyup), all platforms
- [ungit](https://github.com/FredrikNoren/ungit), all platforms
- [LazyGit](https://github.com/jesseduffield/lazygit), all platforms, TUI
- [GitHub CLI](https://cli.github.com), okay a CLI but can be useful for working with GitHub

# Editor Integration
- RStudio: Keefe's notes
- VSCode: [Intro guide](https://code.visualstudio.com/docs/sourcecontrol/intro-to-git)
- Jupyter notebook:
- Vim: [vim-fugitive](https://github.com/tpope/vim-fugitive)
- Emacs: [Magit](https://magit.vc)

# Choosing a Hosting Service (Forge)
- This will be your `remote`
- [GitHub](https://github.com)
- [GitLab](https://about.gitlab.com)
    - [Maynooth GitLab](https://gitlab.cs.nuim.ie) if you're a CS student in Maynooth
- [Gitea](https://about.gitea.com), open source
- [Codeberg](https://codeberg.org), non-profit org for open source
- [SourceHut](https://sourcehut.org), minimal
- Self-host
    - [Forgejo](https://forgejo.org)
    - [Gitea](https://github.com/go-gitea/gitea)
    - [SourceHut](https://sr.ht/~sircmpwn/sourcehut)

# Setting Up a Repo
## Brand New
### Locally
- Demo
- `git init` etc...

### GitHub
- Demo
- Click button

## Existing Project
### Locally
- Demo

### GitHub
- Demo

## Aside: .gitignore
- .gitignore
- .DS_Store
- __pycache__
- Give me some R examples
- Can use wild cards
- Anything generated or too large should be here

# Basic Commands
## Adding
- `git add`

## Diffing
- `git diff`

## Committing
- `git commit`

## Pushing
- `git push`
- Demo

## Surprise aside: SSH keys
- Set them up locally
- Add them to github (or some other remote)
- [GitHub guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?tool=webui&platform=linux)

## Pushing continued
- Follow the git and GitHub instructions!
- `git remote add origin git@github.com:UserName/repo-name.git`
- `git push -u origin main`

## Pulling
- `git pull`
- Demo

## Cloning
- `git clone` url

## Branching
- `git branch name`
- `git switch name`

## Aside: config
- Check mine out in my [dotfiles repo](https://github.com/DaraMac/dotfiles/blob/master/git/.config/git/config)
- Run `git config --list --show-origin` to find out where it is
- `git config --global user.name "Your Name"`


## Merging
<!--TODO: Set up examples here, get them to do it! -->
- Julia's notes
- Demo

## Merge Conflict
- Demo
<!--TODO: Find some diff and merge tools-->
- Manual
- With tool

# Common Problems
- Large file storage
    - What it is, when to use it, how to remove broken things
    - [BFG](https://rtyley.github.io/bfg-repo-cleaner)
- Data storage
    - [datalad.org](https://www.datalad.org)
    - [gin-tonic.netlify.app](https://gin-tonic.netlify.app)
    - [git-annex.branchable.com](https://git-annex.branchable.com)
- Would like to do it automatically, no typing in terminal
- Stash
- Collaboration
- Don't back up .Renviron, from [here](https://bookdown.org/content/d1e53ac9-28ce-472f-bc2c-f499f18264a3/envManagement.html#use-.renviron-file)

