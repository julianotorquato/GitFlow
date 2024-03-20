# GitFlow

![alt text](https://github.com/JfEstrela/GitFlow/blob/master/gitFlow.png)


---

## Main Commands


#### Git global setup

```
git config --global user.name "Your Name"
git config --global user.email "myemail@.com"

```

#### Create a new repository

```
git clone my_uri.git
cd my_uri
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

```


#### Existing folder

```
cd existing_folder
git init
git remote add origin my_uri.git
git add .
git commit -m "Initial commit"
git push -u origin master

git push -u origin master <—force  (not indicated) />

```


#### Existing Git respository

```

cd existing_repo
git remote rename origin old-origin
git remote add origin my_uri.git
git push -u origin --all
git push -u origin --tags

```

#### Cherry Pick

```
git rev-parse d44f865 # convert short hash to commit hash 
git cherry-pick -m 1 833be0ac1ebbf4448a2c24e04432ae523fd4bd06 # get cherry pick when simple command doesn't work cherry-pick xxx "error: commit 5f96728afeb2c8a70405243e78a9b905e29fb8d8 is a merge but no -m option was given."

```

