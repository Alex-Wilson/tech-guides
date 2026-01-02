# Guide to "Git Gud" at Git

## Setting Up Git

## Setting up GitHub CLI 

## Setting up GitHub Account

## Creating a New Repo from Local Folder

0. Create Folder or Navigate to Existing Folder

mkdir $new-folder 

cd $new-folder

or

cd $existing-folder

1. Establish Content
Git requires at least one file (technically file object) to track changes. It cannot track empty folders.  

touch $folder/new-file.txt

2. Local Inititlization and Commit

Initalize the folder with the .git object
git init

Add all files to the repo
git add .

Commit all changes to the repo
git commit -m "initial commit"


3. Create Remote Repository
This can be completed using the "Create Repo" action on the GitHub website or using the "gh" cli. We will use the gh cli. 

gh repo create $repo-name --public --source=$. --remote=origin --push

gh is the name of the command line utility, for help installing it (CLICK HERE)

repo is the action category

create is the action from the repo category, making a new repo

repo-name will be the name of the repository. Ideally this is the name of the folder. 

public indicates anyone with the link will be able to view the entire repository

source indicates that we are generating from an existing directory instead of a blank project. We use "." to indicate the current working directory but this could be replaced with any path.  

remote origin is the secret sauce. It does the "hanshake" for us to ensure that are linking our local directory's changes to the repo on Github. This maps the origin to the URL of the repo created by github when it receives this request. 

push is to send our changes to the newly created repo. 