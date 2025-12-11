 Git & GitHub
---
### What is Git and Github?

> Git
 
- Git is a version control system.
- It tracks changes in your code or files.
- You can go back to previous versions, see history, or work with others safely.
- Works locally on your computer.
- Example: You write a program, then change it. Git lets you save each version so you can return if needed.

> GitHub

- GitHub is an online platform (website) for Git.
- It stores your Git projects in the cloud.
- Lets you share code with others, collaborate, and see projects from other people.
- Think of GitHub as Google Drive for Git projects.

		Git = tool to track code
		GitHub = online place to share and collaborate

<img src="https://github.com/Yacin-lab/Uses/blob/main/img/What-is-Git-repository.webp" width="900" height="800">

### The key Git terms:

- Commit → Save a snapshot of your code. Like a checkpoint.
- Branch → A separate line of work. Lets you try things without breaking main code.
- Merge → Combine a branch back into another branch (usually main).
- Push → Send your changes to GitHub (remote).
- Pull → Get the latest changes from GitHub to your computer.
- Remote repo → The online version of your project (on GitHub).

### Commandes
Clone repo :
```
git clone [path]
```
Add & Reset & Commit :
```
git add [file]
git status
git commit -m "your commit"
git reset [file]
```
Push to remote repo :
```
git branch
git branch -m master main
git remote -v
git push [Remote-name] [Branche-name]
```
Pull Changes (fetch & merge):
```
git fetch
git merge
git pull origin [Branch-name]
```
Create remote repo from command :
```
git init
git remote add origin [remote-repository-url]
```
Configurations :
```
git config -l
git help config
git config --global user.name "Your name"
git config --global user.email "Your_email@example.com"
```
Generate Public Key :
```
ssh-keygen -t rsa -b 4096 -C "Your_email@example.com"
ssh -T git@github.com
```
> [!NOTE]
> #### When connect to GitHub using SSH, GitHub checks:
> - Computer sends a signature using your private key.
> - GitHub compares it with the public key.
> - If they match, GitHub knows it’s really you.

















