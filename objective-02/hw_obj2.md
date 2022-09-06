## Create your own repository

A repository is essentially just a folder on your computer that has a file that tells git that this folder should be treated like a git repository. It can be on your computer or on a website like Github.

Since at Strata we use Github to store our code, I find it easiest to first create the repository on Github directly, and then send it down to your computer.

Go to github.com, log in, and and create a new repository (should be a button either on the github homepage or in your profile, either works)

![image](https://user-images.githubusercontent.com/110128318/188689000-85296835-73b6-4a1b-97d6-3fc06d37aea7.png)

## Clone the repository to your desktop

Next, we have to "clone" that repository down to your desktop, which essentially means downloading it and letting git know that the copy on Github.com is the "origin" we can send changes to. Open git bash (in your VM or windows local) or a terminal (on macOS). For reference, I'm doing this on my VM.

### Navigate to the spot to put your repo

Navigate to a place where you want to put the repository. This should be someplace that's easy to find and access later. I suggest either putting it in your user folder, or a subfolder within your user folder. In git bash the easier way to get there is usually to type `cd $HOME`, cd stands for 'change directory'. You can confirm you're in the right spot with `pwd`, which stands for 'print working directory' and shows you where you are in the folder structure.

![image](https://user-images.githubusercontent.com/110128318/188698350-1f8b34bf-c44d-48c6-9a44-4ab5286965b5.png)

If this does not work because your $HOME variable isn't set up for whatever reason, you can move to a folder directly by typing the full location. If you don't know what your username is, you can cd to the users folder with `cd /c/Users`, then if you do ls (stands for "list") you can see the files in folders in that directory, and then use `cd <your username>` to move into the folder you want.

![image](https://user-images.githubusercontent.com/110128318/188699049-755ea75c-f8e8-43b4-a541-085c4a20d1fe.png)

If you want to make a subfolder to put your git repositories in, you can do that easily on the command line as well with `mkdir`, which stands for "make directory". You can call the folder anything you want. If you go this route, then cd into that directory.

![image](https://user-images.githubusercontent.com/110128318/188699371-f3d38778-5993-402a-9b2b-9a669f44f65e.png)

### Clone the repo

Go to your repository page on Github and click the green "Code" button, and if you're working in the VM, copy the SSH information in the drop down. For this to work you'll need to have the SSH keys part of the VM setup to be complete. If you're not working on the VM but instead your local machine, copy the HTTPS information.

![image](https://user-images.githubusercontent.com/110128318/188745854-212ebafb-8b39-4dd0-a004-a47fd36a20dc.png)

Go back to git bash and do `git clone <insert what you copied>`. To paste into git bash it's usually the shift+insert keys, or right click and choose paste. That should download the directory to that folder. You can then `ls` to see the folder is now there, and `cd` into it.

![image](https://user-images.githubusercontent.com/110128318/188746188-eacd5bfe-69e2-4253-bbee-2115a11f849d.png)

## Create a file in 'main'

In the windows file explorer, find your git repository and create a new text document, call it something like `first_file.txt`. Inside it put some text. Save it. We're going to track these changes with git and push it up to Github.

![image](https://user-images.githubusercontent.com/110128318/188741778-006742c3-887b-41d3-91b8-90dc634ca2c7.png)

## Commit; push changes to Github

In git bash or your terminal, navigate back to your repository if necessary. Then we're going to run `git add first_file.txt`. This will tell git to stage that file to be committed. You have to add the files to be staged first, or else it won't commit the changes you made to that file. If you have many files and you want to add them all, you can use `git add .`, where the period signifies every file in that directory.

Now we're ready to commit. Run `git commit -m 'this is my first commit'`. The -m stands for 'message', and it's one of the options available to the `git commit` command line function, telling git that the string after the -m is a message to describe the commmit. Commit messages are important to understand what was changed in that commit, always add a message. You should see a message that 1 file was changed with 1 insertion.

That change has been saved with a commit on your VM (or wherever you're working). Where it is NOT saved is github... yet. Commits in your repository need to be pushed up to Github explicitly. This is done with `git push`. If you run `git push` it will work, but I also want to point out that we can be more explicit with the command, to tell git where we're trying to push, and what branch (we'll go over branches next) we want to push. With that in mind, run `git push origin main`. This tells git to push to `origin`, which is the default alias of your github repository, and it tells git to push the `main` branch, which is the branch we're currently working on. By default, the first branch created in a Github repository is always called the `main` branch.

If you have your SSH keys setup and you used the SSH information to clone, it should push automatically. If you're using a local machine and HTTPS, you'll have to likely give your credentials (or set up a credential manager) to successfully push to Github.

![image](https://user-images.githubusercontent.com/110128318/188746496-ffd2abe7-ff21-4ae5-b3ac-aa007c39a907.png)

Now if you go to Github and find your repository (refresh if needed), you'll see your commit and file in the repository.

![image](https://user-images.githubusercontent.com/110128318/188746678-e3625f49-8cc2-498c-8504-248b287ca7d1.png)

## Create a branch in git and make another file, commit, push, see new branch in github

Now we're going to create a new branch. A branch is essentially a parrallel (code) universe. If we create a new branch, it's going to be a copy of what `main` currently looks like. We can then make changes and save them as commits in the new branch without affecting `main`. This is really useful when collaborating with others so that you're not overwriting other people's work. Remember, when you're collaborating with other people, you should **always** create a new branch to do your work in, and **never** directly overwrite the `main` branch.

We're going to create a branch called `add-file`. Branch names are arbitrary and descriptive, just call them whatever you want to make it easy for yourself and others to know what the purpose of the branch is. We're going to add another simple text file to the repository, so `add-file` seems appropriate. To do that, run `git branch add-file`, which creates the branch. Then run `git checkout add-file` which switches from the `main` branch to the `add-file` branch. As a shortcut, you might see people just write `git checkout -b add-file` which combines the two steps, creating and checking it out in the same command. It doesn't matter which you use.

You'll see in git bash that the blue indicator text at the end switched from `main` to `add-file`.

![image](https://user-images.githubusercontent.com/110128318/188747858-1be2137b-701d-45c5-ae19-0bbbcc6680e3.png)

Now go add another text file. Call it `second_file.txt` and put in the text `this is my second file, made in the add-file branch`. And now go through the same steps again.

`git add .`

`git commit -m 'adding a second text file'`

`git push origin add-file`

![image](https://user-images.githubusercontent.com/110128318/188754815-6d795387-5a03-48d8-8fc5-05f5868d21fb.png)

And now if we go back to our repository we can see our second branch in the branch drop down, and when we switch to it we can see the new file

![image](https://user-images.githubusercontent.com/110128318/188754979-9bcb83f8-4372-446e-b06a-dd1c6b12200b.png)


## Create pull request

Finally, let's say we accomplished what we want with the second branch and we want to merge our changes back into the `main` branch. That can be done with a pull request, initiated on the Github website.

![image](https://user-images.githubusercontent.com/110128318/188755224-6c2f37cf-695e-4bbf-8415-cc39e2f1fdfa.png)

When you open the pull request you can add a description of what the pull request is, helpful if the maintainer of the project might not know what you're trying to merge in. You can also tag people as code reviewers or assign the pull request to someone. If you're the project owner and you're satisfied with the pull request, you can go ahead and merge the pull request, after which you'll see that if you go back to the main branch, it now has the second text file.

![image](https://user-images.githubusercontent.com/110128318/188755511-b7ae83ad-34ee-4463-b5f8-21544d90bf2b.png)

After merging, you can delete the branch in Github if you want to keep the project cleaner and more organized, since you presumably don't need that branch anymore.

Finally, if you want those changes reflected on your local copy, you'll have to run `git pull` on the command line to pull down all the latest changes that happened on Github, in this case, the merge that occured from the pull request.
