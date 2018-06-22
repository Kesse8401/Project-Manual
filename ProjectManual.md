#PROJECT MANUAL#

##1.Setting a new Project##

*TERMINAL*: 	Open terminal, navigate to right place (eg. cd Desktop/Projects) and create new folder: mkdir newFolderName, then enter in to the new foleder (cd Desktop/Projects/newFolderName) then it’s good to create to basic files: touch index.html and touch README.md
Next a local repository should be created: git init

*SOURCE TREE*: On the main dashboard click NEW (with the dropdown) anch choose Add existing local repository,  (choose a folder, not a file) then double-click on the repository that shows in the window.
Than stage all files by marking (ptaszkiem) and press button COMMIT. Make sure to provide descriptive name.
Right-click on a REMOTE and choose new remote (first remote is always called origin)
Add URL (copied from GitHub and make sure is by SSH not HTTPS). Click on REMOTe and choose show than choose FETCH (from all remotes) and OK.
Next, find the last commit, go to workspace, then history and use button PUSH to connect your local repo with gitHub.

When using new computer/system you might need to add local key from my computer to my repo. You can do that by going to main gitHub settings, choose SSH and GPR keys, choose New SSH Keys and add new (with title). There is a guide on gitHUb how to do it (https://help.github.com/articles/signing-commits-with-gpg/)  but essentially file id_rsa.pub needs to be save and then (on terminal) use commend cat d_rsa.pu.  Copy, save and paste as a new SSH key in gitHub

*GIT HUB*: Log in and create New Repo by clicking on +. Copy a link assigned to that repo.


##2. Making changes in files##

*VSC*: After making change to a file(s) they need to be staged: by clicking in to source control, and clicking small + next to file(s) that was changed. Once it has been staged it can be committed by (ptaszek). It requires name that should descriptively explain nature of change an #number referring to equivalent issue/stage in gitHUb.
Once the changes are committed, they need to be pushed. It can be achieved from VSC* by making sure that in a lower left corner, right branch is chosen and than clicking on the ↑ with the number (of stage files) next to it.

*SOURCE TREE*: staging and pushing can be also done from SourceTree. Simply find the last commit, go to workspace, then history and use button PUSH


##3.Creating new branch##

Creating new branch is necessary for person/people to work on progressing project without negatively affecting main version (master branch) of the project.
To create new branch go to

*SOURCE TREE*: right click on branch, choose add new and name it (in a descriptive way). Than in a text editor make sure you working on/making changes/staging/commiting/pushin to the right branch.

##4. Pull Request##

Pulling a request is a good idea after staging significant changes to the branch, so other people could see what have changed and comment on it. As pull requests are created, they’ll appear here in a searchable and filterable list. To get started, you should create a pull request.
The New Pull Request button can be found in Pull Request tab in gitHub.


##5. Requirements of every project##

Every project required installing/adding several files/modules:

*.gitignore* it is a file that specifies which elements of a project should not be pushed to git, as to not repeat the pieces of code. Good templates of gitignore file contents can be found on: https://www.gitignore.io/ (make sure to give some details such as name of your text editor, used modules, language)

*package.json* is one of the most important files in a project. It contains all informations such as name, version, name and link to a repository, name of the author, type of licence and all dependencies and devDependencies. In order to create default file cd to you program root folder (eg. Desktop/Projects/newFolderName) in terminal and add command npm init. After enter terminal will ask as questions/confirmations. Default answers are in parenthesis. If we would like to change any/all of those we should type in correct version and press enter.
If we would like to change something afterwards we should go to terminal, and use command: 
npm config set init-author-name “some name”, than delete package.json form text editor and put command npm init -y
If we would like to blindly accept all defaults right command on terminal is npm init --y or npm init -y.

*node_modules* is an external, npm folder filled with useful modules that will help to execute a project.
To install it globally (on the computer):

To install it locally (only with attachment to the project)

*Package-lock.json* siusiak jeden wie co to jest, po co i jak to zainstalować… mi się to pojawiło przy okazji!

*README.md* is a file describing the project with details such as what does it do and how to installed. Good template of readme.md file can be found here: https://gist.github.com/PurpleBooth/109311bb0361f32d87a2




