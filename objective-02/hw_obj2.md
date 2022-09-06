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

Go to your repository page on Github and click the green "Code" button, copy the HTTPS information in the drop down

![image](https://user-images.githubusercontent.com/110128318/188696802-98636026-cdd0-4a89-bd9d-0e2f28976c3a.png)

Go back to git bash and do `git clone <insert what you copied`, to paste into git bash it's usually the shift+insert keys, or right click and choose paste. That should download the directory to that folder. You can then `ls` to see the folder is now there, and `cd` into it.

![image](https://user-images.githubusercontent.com/110128318/188700395-5d62019d-39a4-43ed-bca2-7cc6e0fcf5fc.png)


## Create a file in 'main'

## Commit, push changes to Github

## Create a branch in git and make another file

## Commit, push changes to Github, see the other branch in Github

## Create pull request
