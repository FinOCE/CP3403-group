# CP3403 Assignment

## Group members:

- Jarred Muller
- Naoki Da Costa
- Daniel Mackenzie
- Finley Sherwood

## Guide to committing changes

There may be some situations where issues happen, but I believe this should be the way for us to all work on the same repository.

### Create your local repo

If you haven't yet, create a folder to store the local repository. You can do this manually in your file explorer or run the following in the console:

```shell
cd your/project/parent/directory
mkdir cp3403-group
cd cp3403-group
```

Once you have the folder created, setup the repository.

```shell
git init
git remote add origin https://github.com/FinOCE/CP3403-group.git
```

### Pushing changes to the shared repo

Steps from here on need to be done every time you wish to work on the repo. Once you have completed your merge you restart from here to ensure you are pushing to the correct place.

```shell
git pull origin main
git checkout -b finley # Replace with your name

# If you're working with VSCode and are running these commands from a separate terminal, you can use below to open it in the program
code .
```

From here you are working on your local personal branch. Make changes and commits as you normally would (I recommend just using the VSCode source control GUI for this stuff). Once you've finished with your work, press the button "Publish Branch" that shows there. This button pushes the branch to Github, so it is visible to everyone online.

Go to [the repo branches page](https://github.com/FinOCE/CP3403-group/branches) and press "New pull request" next to your branch. Assuming there are no conflicts, you should be able to then just merge the branch. If there are any conflicts, please let me know and I will have a look and try sort them out.

Once the branch has been merged, you can then delete the branch from that same branches page, since all updates are now in the main branch. To remove the branch from your local repo, run this:

```shell
git checkout main
git branch -d finley # Replace with your name
```

If you want to then do more work on it another time, simply start again from the start of this section (Pushing changes to the shared repo) and repeat the steps.
