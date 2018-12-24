# Uploading your project to GitHub

## Step 1: Planning the move

介绍了使用GitHub的好处和一些准备工作，无其他操作步骤。

close issue 进入step 2。

## Step 2: Prepare the project

### Working with Binary files

使用 [git-lfs](https://git-lfs.github.com/) (Git Large File Storage)来管理二进制文件。

### Add a .gitignore

为你要上传的仓库添加[`.gitignore` 文件](https://help.github.com/articles/ignoring-files/)。参考[`github/gitignore`](https://github.com/github/gitignore) 模版来添加。

### Activity: Prepare your repository

1. 移除仓库里所有二进制文件

2. 在仓库里添加`.gitignore`文件

close issue 进入step 3。

## Step 3: Make the move

###  Activity: Moving your local project

打开`Code`标签，复制`Quick Setup` 后面的  URL（`https://github.com/用户名/github-upload.git`）。

### 命令行

在仓库目录里打开命令行,输入下面的命令：

    git init
    git remote add origin https://github.com/copyshiroe/github-upload.git
    git add .
    git commit -m "initializing repository"
    git push -u origin master


### Visual Studio Code

1. In Visual Studio Code, open the folder for your project.
2. Click the icon on the left for `Source Control`.
3. On the top of the `Source Control panel`, click the `Git icon`.
4. If the files you see match the repository you want to create, click `Initialize Repository`.
5. Next to the word `CHANGES`, click the symbol of the plus sign to stage all of the changes.
    - This is part of the two stage commit. You can use this staging function to create meaningful commits throughout the development process.
6. In the box in the `Source Control panel`, type a commit message. Something like "initial commit - moving project" could work.
7. Click the **checkmark** at the top of the `Source Control panel`.
8. Open the integrated terminal found under `View > Integrated Terminal`.
9. In your command line, type `git remote add origin`
10. In the `Source Control Panel`, click the expandable three dots that open a menu of options.
11. When asked if you'd like to publish the branch, click `Okay`.



### Using Atom

1. In Atom, open the folder for your project
2. At the top of your screen, click **Packages**. Select **GitHub**, and then toggle the **Git Tab** from the drop-down menu.
3. Select **Create Repository** within the Git tab on the right-hand size of your screen.
4. Select **Init** to accept the default prompt of the pop up window
5. In the Git tab, you can see that your files are ready for staging. It *should* be accounted for, but double check to make sure that none of your binaries or files that you listed in the .gitignore are listed in this dialog menu.
	\- If they are, double check your .gitignore file to make sure they're included or remove them from your directory.
6. Select **Stage All**
	\- This is part of the two stage commit. You can use this staging function to create meaningful commits throughout the development process.
7. In the box at the bottom of the Git panel, type a commit message. Something like "initial commit - moving project" could work.
8. Select **Commit**
9. Close Atom
10. In your command line, navigate to your project directory.
11. Type `git remote add origin`
12. Return to Atom, and select the [Up/Down arrow icon](https://user-images.githubusercontent.com/13326548/36766999-34ff2bb2-1bed-11e8-90c6-3c97d0837244.png) at the bottom of your Git Tab
13. Click [Push](https://user-images.githubusercontent.com/13326548/36767211-5fd34ce6-1bee-11e8-964a-f49bed227c02.png), above the noted dialog.
14. Return to your repository, and note a successful push by finding your files on GitHub's code tab



### Using Eclipse

1. In Eclipse, from the Eclipse Marketplace, install the [eGit](http://www.eclipse.org/egit/) GitHub plugin.
2. Open your existing project.
3. Display the `Git Repositories` window by selecting `Window > Show View > Other > Git > Git Repositories`.
4. Click the `Create a Git Repository` button on the `Git Repositories pane`.
5. Make changes to your project and create a commit.
6. Push the master branch.
7. When asked for a remote, paste the URL you copied earlier.
8. Click next, and enter the branch name.



推送完仓库后进入下一步。


