## Git
Git is the most popular version control system. A version control system tracks and records changes made in our code over time in a special hidden folder created in the project directory called a repository. Git help us check project history to know what was changed, when and by who. This helps developers to scale, collaborate and work together seemlessly. In addition, it is important to be aware that before git can be used on your local machine, it has to be installed.

## Repository
A git repository is a hidden directory created in our project directory. It is the `.git/` folder inside your project directory. The repository tracks all changes to build a history over time. All this changes are tracked and stored locally in your machine.
It is important to note that this .git/ folder known as the repository doesn't appear untill it is initialized using git. There's a number of ways to initialize a git repository. One way is by using the terminal. To initialized a git repository using the terminal, simply run `git init`.

## Remote
This is also known as "Remote Repository". It is a git repository hosted on the internet. After using git to initialize a repository to track project changes on your local machine, you can equally create a repository on Github hosted on the internet. Git enables us to link the repository present in our local machine to the repository hosted on the internet allowing `push` and `pull` actions with the remote project.

This has alot of advantages, one major advantage is that it stores your project on the internet, now you can access and make changes to your project with or without the computer you used to start the project. 

## Branching
Branching is how git enable multiple developers to collaborate and work on a project by modifying the working codebase. When you create a branch, git creates a different codebase where you can make changes and modify files without affecting the main codebase which is usually on the main branch. A branch can be created using the terminal by running `git branch <new_branch_name>`.

## Merging
Once you’ve completed work on your branch, you can decide to merge it with the main branch. Merging simply means updating the main branch with changes from another branch in the same repository. When the `git merge <branch_name>` command is run, git scans through your branch for changes and updates the main (main branch) with found changes. 

## Merge Conflicts
Sometimes merging a branch to the main isn't as straight forward as writing a single command on the terminal. In a scenerio where two developers are working on the same file in a project from different branches, the first merge from the first branch might have no conflict but when you try to merge the second branch, there will be a merge conflict especially when both branches modified the same file. Reason for the conflict is that git doesn't know which version of the file to keep. Everytime there's a merge conflict, git shows you every line of code that has a conflict and you'll have to manually decide which part of the code stays and which goes. While resolving merge conflict on the terminal, it is important that you delete the merge markers along side the unwanted code.

## The three git states
Growing up, my mum gave me a job. She would always give some money to me to save in a piggybank (Kolo, as we locally call it) almost everyday as she returns from work. On Friday I would take the kolo into a bank, round up the money and deposit it. Git states works in a similar way.

### Modified
This means there's new file(s) or new changes that is not tracked by git. It is that straight forward. Using my analogy, think of my mum as a developer and I as git except instead of tracking and managing code, it's money. When my mum comes back from work, whether or not she has some change to save, I wouldn't know unless she calls me and tell me so. Same goes for git, git won't track your changes until you tell it to do so.

### Staging
This is also called index. This means git is now aware of the new changes and can now track the file(s). You can take your code to the staging area by runing `git add file1`. This means that file1 is now tracked and it's changes is ready to be commited. Back to my analogy again. This stage is where my mum delivers the money into my hands after work, now I am aware of the new input and I can record it.

### Committed
This takes the current state of the code, the person who made the change, the time, commit message and store it in the git repository like a snapshot with a unique commit ID. This help us track project history and prepare the code to be pushed to the remote. Based on the analogy, committed is related to the money that has made it into the Kolo (piggybank) ready to visit the bank on Friday.



[Here's a link to a video on Youtube to help you understand better](https://www.youtube.com/watch?v=8JJ101D3knE)
