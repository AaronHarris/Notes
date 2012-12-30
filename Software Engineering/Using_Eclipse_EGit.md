Using Eclipse EGit
=====

So setting up Git for Eclipse doesn't seem to be so hard after all.

##Setting Up
1. Go to **Help \> Install New Software**
2. Under the **Work with:** drop down, select `Juno - http://download.eclipse.org/releases/juno`
3. Type in "Git" in filter text, select **Eclipse EGit**, **Eclipse JGit**
4. Follow the instructions, then restart Eclipse
5. Go to **Window \> Show View \> Other**, filter "Git", and add _Git Repositories_.
6. In that new panel opened, choose either of the 3rd or 4th option on the toolbar, based on how your existing system is set up.
    * Add an existing Git repository - you can have Eclipse reference to that repo, and not change anything of what you've checked out already.
    * Clone a Git Repository to check out another repository to your workspace
7. Open the "[name_of_repo]" tree, right click on the folder containing the Eclipse project, and select **Import Projects**.
8. In the pop-up, select "[name_of_project]", and follow the instructions to finish.

## Committing Changes
There are three ways to do this.

### Continue what you do best.
Just make your changes, and commit / sync via the Git command line.

### Git Repositories
After finishing your changes, right click on _[repo_name]_ under the Git Repositories panel, and select **Commit**. Follow the steps, and make sure you have "push to upstream" selected.

### Git Staging
1. Go to **Window \> Show View \> Other**, filter "Git", and add _Git Staging_.
2. Any changes you've made will be shown in the list of files under _Unstaged Changes_. You need to drag them to _Staged Changes_.
3. Put in a commit message
4. Press the **Commit button** on top right of panel.
5. Push, under the _Git Repositories_ panel.
