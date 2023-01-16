# Creating a Local Repository and Pushing it to GitHub

1. Open a terminal window and navigate to the directory where you want to create your repository.

2. Initialize a new Git repository by running the command:

```c
git init

```

3. Add the files you want to track in your repository using the command:

```c
git add .

```

This command will add all the files in the current directory to the repository. If you want to add specific files, you can use `git add file1 file2`

4. Commit the added files to the repository by running the command:

```c
git commit -m "Initial commit"

```

This command will create the first commit in the repository with the message "Initial commit"

5. Now, create a new repository on GitHub by visiting the GitHub website and clicking on the "+" button in the top-right corner, then selecting "New repository". Give it a name and select the public or private option.

6. Once the repository is created, you will see the URL of the repository on the repository page.

7. Now link your local repository with the remote repository by running the command:

```c
git remote add origin <repository_url>

```


8. Finally, push the local repository to the remote repository by running the command:

```c
git push -u origin master

```


This command will push the master branch of the local repository to the remote repository.

Please note that, if the repository is private, you will need to configure your ssh-key or credentials to push the repository.

check this [GITHUBAPI](githubApI/README.md)
 see how to get a github api key.

You can check the status of the repository by running `git status`, you can see the logs by running `git log` and you can see the remote repository details by running `git remote -v`

You can also use Git GUI client tools like SourceTree, GitKraken etc which will make the process of creating, committing and pushing to the repository easier.





